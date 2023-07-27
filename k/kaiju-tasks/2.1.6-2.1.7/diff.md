# Comparing `tmp/kaiju_tasks-2.1.6-py3-none-any.whl.zip` & `tmp/kaiju_tasks-2.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 17698 bytes, number of entries: 12
--rw-r--r--  2.0 unx      150 b- defN 23-Jul-16 15:12 kaiju_tasks/__init__.py
--rw-r--r--  2.0 unx     5386 b- defN 23-Jul-16 15:12 kaiju_tasks/gui.py
--rw-r--r--  2.0 unx    38123 b- defN 23-Jul-16 15:12 kaiju_tasks/services.py
--rw-r--r--  2.0 unx     4425 b- defN 23-Jul-16 15:12 kaiju_tasks/types.py
--rw-r--r--  2.0 unx       42 b- defN 23-Jul-16 15:12 kaiju_tasks/tests/__init__.py
--rw-r--r--  2.0 unx     2272 b- defN 23-Jul-16 15:12 kaiju_tasks/tests/fixtures.py
--rw-r--r--  2.0 unx    12861 b- defN 23-Jul-16 15:12 kaiju_tasks/tests/test_tasks.py
--rw-rw-rw-  2.0 unx      610 b- defN 23-Jul-16 15:12 kaiju_tasks-2.1.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     3206 b- defN 23-Jul-16 15:12 kaiju_tasks-2.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-16 15:12 kaiju_tasks-2.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jul-16 15:12 kaiju_tasks-2.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      976 b- defN 23-Jul-16 15:12 kaiju_tasks-2.1.6.dist-info/RECORD
-12 files, 68155 bytes uncompressed, 16060 bytes compressed:  76.4%
+Zip file size: 18801 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      151 b- defN 23-Jul-27 19:42 kaiju_tasks/__init__.py
+-rw-r--r--  2.0 unx     5386 b- defN 23-Jul-27 19:42 kaiju_tasks/gui.py
+-rw-r--r--  2.0 unx    40431 b- defN 23-Jul-27 19:42 kaiju_tasks/services.py
+-rw-r--r--  2.0 unx     6161 b- defN 23-Jul-27 19:42 kaiju_tasks/types.py
+-rw-r--r--  2.0 unx       42 b- defN 23-Jul-27 19:42 kaiju_tasks/tests/__init__.py
+-rw-r--r--  2.0 unx     2272 b- defN 23-Jul-27 19:42 kaiju_tasks/tests/fixtures.py
+-rw-r--r--  2.0 unx    15554 b- defN 23-Jul-27 19:42 kaiju_tasks/tests/test_tasks.py
+-rw-rw-rw-  2.0 unx      610 b- defN 23-Jul-27 19:43 kaiju_tasks-2.1.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3212 b- defN 23-Jul-27 19:43 kaiju_tasks-2.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-27 19:43 kaiju_tasks-2.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jul-27 19:43 kaiju_tasks-2.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      976 b- defN 23-Jul-27 19:43 kaiju_tasks-2.1.7.dist-info/RECORD
+12 files, 74899 bytes uncompressed, 17163 bytes compressed:  77.1%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: kaiju_tasks/tests/fixtures.py
 Comment: 
 
 Filename: kaiju_tasks/tests/test_tasks.py
 Comment: 
 
-Filename: kaiju_tasks-2.1.6.dist-info/LICENSE
+Filename: kaiju_tasks-2.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_tasks-2.1.6.dist-info/METADATA
+Filename: kaiju_tasks-2.1.7.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_tasks-2.1.6.dist-info/WHEEL
+Filename: kaiju_tasks-2.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_tasks-2.1.6.dist-info/top_level.txt
+Filename: kaiju_tasks-2.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_tasks-2.1.6.dist-info/RECORD
+Filename: kaiju_tasks-2.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_tasks/__init__.py

```diff
@@ -1,7 +1,7 @@
 from .types import *
 from .services import *
 from .gui import *
 
-__version__ = '2.1.6'
-__python_version__ = '3.8'
+__version__ = '2.1.7'
+__python_version__ = '3.11'
 __author__ = 'antonnidhoggr@me.com'
```

## kaiju_tasks/services.py

```diff
@@ -1,45 +1,49 @@
 """Services and classes."""
 
-from enum import Enum
 from datetime import datetime, timedelta, timezone
+from enum import Enum
 from time import time
-from uuid import uuid4, UUID
 from typing import Any, List
+from uuid import UUID, uuid4
 
+import kaiju_tools.jsonschema as j
 import sqlalchemy as sa
 import sqlalchemy.dialects.postgresql as sa_pg
 from croniter import croniter
-
-import kaiju_tools.jsonschema as j
-from kaiju_tools.app import ContextableService, Scheduler, SERVICE_CLASS_REGISTRY
-from kaiju_tools.exceptions import ValidationError, InternalError
-from kaiju_tools.interfaces import PublicInterface
+from kaiju_db import DatabaseService, PermHook, SQLService
+from kaiju_redis import RedisTransportService
+from kaiju_tools.app import SERVICE_CLASS_REGISTRY, ContextableService, Scheduler
+from kaiju_tools.exceptions import InternalError, ValidationError
 from kaiju_tools.functions import get_short_uid, retry
+from kaiju_tools.interfaces import PublicInterface
+from kaiju_tools.rpc import JSONRPCHeaders, JSONRPCServer, RPCError
 from kaiju_tools.streams import StreamRPCClient, Topic
 from kaiju_tools.templates import Template
-from kaiju_tools.rpc import JSONRPCServer, JSONRPCHeaders, RPCError
 from kaiju_tools.types import Scope
-from kaiju_db import SQLService, DatabaseService
-from kaiju_redis import RedisTransportService
 
-from kaiju_tasks.types import TaskStatus, RestartPolicy, Limit, Task, ExecutorTask, Notification, TaskCommand
+from kaiju_tasks.types import (
+    ExecutorTask,
+    Limit,
+    Message,
+    Notification,
+    RestartPolicy,
+    Task,
+    TaskCommand,
+    TaskStatus,
+    Timer,
+)
+
 
 __all__ = ['TaskService', 'NotificationService', 'TaskManager', 'TaskExecutor']
 
 
-class TaskService(SQLService[str, Task], PublicInterface):
+class TaskService(SQLService[str, Task], PermHook, PublicInterface):
     """Tasks public interface.."""
 
-    class Permission(Enum):
-        """Task service special permission keys."""
-
-        VIEW_OTHERS_TASKS = 'tasks.view_other_tasks'
-        MODIFY_OTHERS_TASKS = 'tasks.modify_others_tasks'
-
     service_name = 'tasks'
     table = sa.Table(
         'tasks',
         sa.MetaData(),
         sa.Column('id', sa_pg.TEXT, primary_key=True),
         # executor instructions
         sa.Column('app_name', sa_pg.TEXT, nullable=False),
@@ -61,33 +65,47 @@
         sa.Column('status', sa_pg.TEXT, nullable=False),
         sa.Column('result', sa_pg.JSONB, nullable=False),
         sa.Column('stage', sa_pg.INTEGER, nullable=False),
         sa.Column('stages', sa_pg.INTEGER, nullable=False),
         sa.Column('created', sa_pg.TIMESTAMP(timezone=True), nullable=False),
         sa.Column('queued_at', sa_pg.INTEGER, nullable=True),
         sa.Column('exec_deadline', sa_pg.INTEGER, nullable=True),
+        sa.Column('wait_deadline', sa_pg.INTEGER, nullable=True),
         sa.Column('next_run', sa_pg.INTEGER, nullable=True),
         sa.Column('user_id', sa_pg.UUID(as_uuid=True), nullable=True),
         sa.Column('executor_id', sa_pg.UUID(as_uuid=True), nullable=True),
         sa.Column('job_id', sa_pg.TEXT, nullable=True),
         sa.Column('retries', sa_pg.INTEGER, nullable=False),
         sa.Column('exit_code', sa_pg.INTEGER, nullable=True),
         sa.Column('error', sa_pg.JSONB, nullable=True),
     )
-    sa.Index(f'idx__{table.name}__queued_at', table.c.queued_at.desc(), postgresql_where=table.c.enabled.is_(True))
-    sa.Index(f'idx__{table.name}__next_run', table.c.next_run.desc(), postgresql_where=table.c.enabled.is_(True))
+    sa.Index(
+        f'idx__{table.name}__queued_at',
+        sa.nulls_last(sa.desc(table.c.queued_at)),
+        postgresql_where=table.c.enabled.is_(True),
+    )
+    sa.Index(
+        f'idx__{table.name}__wait_deadline',
+        sa.nulls_last(sa.desc(table.c.wait_deadline)),
+        postgresql_where=table.c.enabled.is_(True),
+    )
+    sa.Index(
+        f'idx__{table.name}__next_run',
+        sa.nulls_last(sa.desc(table.c.next_run)),
+        postgresql_where=table.c.enabled.is_(True),
+    )
     sa.Index(
         f'idx__{table.name}__cron',
         table.c.cron,
-        postgresql_where=sa.and_(table.c.cron.isnot(None), table.c.enabled.is_(True)),
-    )  # TODO: is_not for alchemy 1.4
+        postgresql_where=sa.and_(sa.not_(table.c.cron.is_(None)), table.c.enabled.is_(True)),
+    )
     sa.Index(
         f'idx__{table.name}__status__idle',
-        table.c.next_run.desc(),
-        postgresql_where=sa.and_(table.c.enabled.is_(True), table.c.status == TaskStatus.IDLE.value),
+        sa.nulls_last(sa.desc(table.c.next_run)),
+        postgresql_where=table.c.enabled.is_(True),
     )
 
     _task_command = j.Object(
         {'id': j.Integer(), 'method': j.String(), 'params': j.Object()}, additionalProperties=False, required=['method']
     )
 
     _task_validator = j.Object(
@@ -109,37 +127,42 @@
         },
         additionalProperties=False,
         required=['commands'],
     )
 
     @property
     def routes(self) -> dict:
-        return {**super().routes, 'reset': self.reset_task, 'delete_old_tasks': self.delete_old_tasks}
+        return {
+            **super().routes,
+            'reset': self.reset_task,
+            'delete_old_tasks': self.delete_old_tasks,
+            'write_message': self.write_message,
+        }
 
     @property
     def permissions(self) -> dict:
         return {
             '*': self.PermissionKeys.GLOBAL_USER_PERMISSION,
             'delete_old_tasks': self.PermissionKeys.GLOBAL_SYSTEM_PERMISSION,
         }
 
     @property
     def validators(self) -> dict:
         return {'create': j.Object({'data': self._task_validator}, additionalProperties=True, required=['data'])}
 
     async def delete_old_tasks(self, interval_days: int = 7) -> None:
         """Delete old tasks and notifications (excluding periodic and system tasks)."""
-        sql = self.table.delete().where(
-            sa.and_(
-                self.table.c.cron.is_(None),
-                self.table.c.created < datetime.now() - timedelta(days=interval_days),
-                self.table.c.system.is_(False),
-            )
+        await self.m_delete(
+            conditions={
+                'cron': None,
+                'created': {'lt': datetime.now() - timedelta(days=interval_days)},
+                'system': False,
+            },
+            columns=[],
         )
-        await self._wrap_delete(None, sql)
 
     async def reset_task(self, id: str) -> bool:
         """Reset task to IDLE and remove result / errors.
 
         :returns: True if task has been restarted, False if it can't be restarted
         """
         restarted = await self.m_update(
@@ -148,21 +171,43 @@
                 'status': TaskStatus.IDLE.value,
                 'executor_id': None,
                 'job_id': get_short_uid(),
                 'exit_code': None,
                 'error': None,
                 'retries': 0,
                 'exec_deadline': None,
+                'wait_deadline': None,
                 'stage': 0,
                 'result': [],
             },
             columns=['id'],
         )
         return bool(restarted)
 
+    async def write_message(self, id: str, data: dict) -> bool:
+        """Send a message to a task which must be in a 'WAITING' state.
+
+        The task will be rescheduled for execution from the next stage. Message will be available
+        in the task results.
+
+        :returns: True if a task has received the message
+        """
+        updated = await self.m_update(
+            id=[id],
+            data={
+                'status': TaskStatus.SUSPENDED.value,
+                'result': self.table.c.result + [data],
+                'stage': self.table.c.stage + 1,
+                'executor_id': None,
+            },
+            conditions={'status': TaskStatus.WAITING.value},
+            columns=['id'],
+        )
+        return bool(updated)
+
     def prepare_insert_data(self, data: dict):
         """Prepare task."""
         data = self._validate_data(data)
         task = Task(
             id=data.get('id', str(uuid4()).replace('-', '')),
             app_name=data.get('app', self.app.name),
             commands=[TaskCommand(method=cmd['method'], params=cmd.get('params')) for cmd in data['commands']],
@@ -179,14 +224,15 @@
             status=TaskStatus.IDLE.value,
             stage=0,
             stages=len(data['commands']),
             result=[],
             created=sa.func.now(),
             queued_at=None,
             exec_deadline=None,
+            wait_deadline=None,
             next_run=int(time()),
             user_id=self.get_user_id(),
             executor_id=None,
             job_id=get_short_uid(),
             retries=0,
             exit_code=None,
             error=None,
@@ -203,39 +249,19 @@
         if cron:
             croniter(data.get('cron'), start_time=datetime.now()).next()  # testing for validity
         commands = data.get('commands')
         if commands and len(commands) == 0:
             raise ValidationError('Commands must not be empty.')
         return data
 
-    def _set_user_condition(self, sql, permission: str):
-        """Places user condition if a user has no admin/system privileges."""
-        if not self.has_permission(permission):
-            user_id = self.get_user_id()
-            sql = sql.where(self.table.c.user_id == user_id)
-        return sql
-
-    def _get_condition_hook(self, sql):
-        return self._set_user_condition(sql, self.Permission.VIEW_OTHERS_TASKS.value)
 
-    def _update_condition_hook(self, sql):
-        return self._set_user_condition(sql, self.Permission.MODIFY_OTHERS_TASKS.value)
-
-    def _delete_condition_hook(self, sql):
-        return self._update_condition_hook(sql)
-
-
-class NotificationService(SQLService[UUID, Notification], PublicInterface):
+class NotificationService(SQLService[UUID, Notification], PermHook, PublicInterface):
     """Task notifications interface."""
 
-    class Permission(Enum):
-        """Notification service special permissions."""
-
-        VIEW_OTHERS_NOTIFICATIONS = 'notifications.view_others_notifications'
-        MODIFY_OTHERS_NOTIFICATIONS = 'notifications.edit_others_notifications'
+    service_name = 'notifications'
 
     table = sa.Table(
         'notifications',
         sa.MetaData(),
         sa.Column('id', sa_pg.UUID(as_uuid=True), primary_key=True, server_default=sa.text('uuid_generate_v4()')),
         sa.Column('task_id', sa.ForeignKey(TaskService.table.c.id, ondelete='CASCADE'), nullable=True),
         sa.Column('message', sa_pg.TEXT, nullable=True),
@@ -246,37 +272,18 @@
         sa.Column('user_id', sa_pg.UUID(as_uuid=True), nullable=True),
         sa.Column('job_id', sa_pg.TEXT, nullable=True),
         sa.Column('status', sa_pg.TEXT, nullable=True),
         sa.Column('result', sa_pg.JSONB, nullable=True),
         sa.Column('exit_code', sa_pg.INTEGER, nullable=True),
         sa.Column('error', sa_pg.JSONB, nullable=True),
     )
-    sa.Index('idx_notification_timestamp', table.c.user_id, table.c.created.desc())
+    sa.Index('idx_notification_timestamp', table.c.user_id, sa.desc(table.c.created))
 
-    service_name = 'notifications'
     update_columns = {'enabled'}
 
-    def _set_user_condition(self, sql, permission: str):
-        """Places user condition if a user has no admin/system privileges."""
-        if not self.has_permission(permission):
-            user_id = self.get_user_id()
-            sql = sql.where(self.table.c.user_id == user_id)
-        return sql
-
-    def _update_condition_hook(self, sql):
-        """Places user condition if a user has no admin/system privileges for editing all the data."""
-        return self._set_user_condition(sql, self.Permission.MODIFY_OTHERS_NOTIFICATIONS.value)
-
-    def _delete_condition_hook(self, sql):
-        return self._update_condition_hook(sql)
-
-    def _get_condition_hook(self, sql):
-        """Places user condition if a user has no admin/system privileges for viewing all the data."""
-        return self._set_user_condition(sql, self.Permission.VIEW_OTHERS_NOTIFICATIONS.value)
-
 
 class TaskManager(ContextableService, PublicInterface):
     """Task manager which schedules tasks execution."""
 
     class ExitCode(Enum):
         """Default task unix style exit codes."""
 
@@ -330,14 +337,16 @@
     def routes(self) -> dict:
         return {
             'list_active_executors': self.list_active_executors,
             'ping': self.ping,
             'suspend_executor': self.suspend_executor,
             'execute_stage': self.execute_stage,
             'write_stage': self.write_stage,
+            'wait_for_message': self.wait_for_message,
+            'wait_for_timer': self.wait_for_timer,
             'cleanup': self.cleanup,
         }
 
     @property
     def permissions(self) -> dict:
         return {'*': self.PermissionKeys.GLOBAL_SYSTEM_PERMISSION}
 
@@ -410,35 +419,67 @@
                     'executor_id': executor_id,
                 }
             )
         )
         await self._db.execute(sql)
         await self.ping(executor_id)
 
+    async def wait_for_timer(self, task_id: str, executor_id: UUID, stage: int, deadline: int) -> None:
+        """Require a task to wait for a message to continue."""
+        sql = (
+            self.table.update()
+            .where(
+                sa.and_(
+                    self.table.c.id == task_id,
+                    self.table.c.status == TaskStatus.EXECUTED.value,
+                    self.table.c.executor_id == executor_id,
+                )
+            )
+            .values(
+                {'status': TaskStatus.WAITING.value, 'stage': stage, 'executor_id': None, 'wait_deadline': deadline}
+            )
+        )
+        await self._db.execute(sql)
+
+    async def wait_for_message(self, task_id: str, executor_id: UUID, stage: int) -> None:
+        """Require a task to wait for a message to continue."""
+        sql = (
+            self.table.update()
+            .where(
+                sa.and_(
+                    self.table.c.id == task_id,
+                    self.table.c.status == TaskStatus.EXECUTED.value,
+                    self.table.c.executor_id == executor_id,
+                )
+            )
+            .values({'status': TaskStatus.WAITING.value, 'stage': stage, 'executor_id': None})
+        )
+        await self._db.execute(sql)
+
     async def write_stage(
         self, task_id: str, executor_id: UUID, stage: int, stages: int, result: Any, error: bool
     ) -> None:
         """Write stage result to the task table.
 
         This method will also change task status depending on which stage has been executed. The task my become
         'FINISHED' or 'FAILED'.
         """
         sql = self.table.update().where(
             sa.or_(
                 sa.and_(
                     self.table.c.id == task_id,
                     self.table.c.executor_id == executor_id,
                     self.table.c.stage == stage,
-                    self.table.c.status.in_([TaskStatus.EXECUTED.value]),
+                    self.table.c.status == TaskStatus.EXECUTED.value,
                 ),
                 sa.and_(
                     self.table.c.id == task_id,
                     self.table.c.executor_id.is_(None),
                     self.table.c.stage == stage,
-                    self.table.c.status.in_([TaskStatus.QUEUED.value]),
+                    self.table.c.status == TaskStatus.QUEUED.value,
                 ),
             )
         )
         columns = [self.table.c.job_id, self.table.c.result, self.table.c.notify, self.table.c.user_id]
         if error:
             sql = sql.values(
                 {
@@ -519,14 +560,15 @@
                 self.logger.info('Stage finished', stage=stage, task_id=task_id, executor_id=executor_id)
 
     async def _queue_tasks(self):
         """Iterate over the tasks table."""
         await self._expell_dead_executors()
         await self._abort_timed_out_tasks()
         await self._restart_cron_tasks()
+        await self._queue_timers()
         await self._queue_suspended_and_idle()
         await self._queue_failed()
 
     async def _expell_dead_executors(self):
         """Check if some executors are not responding and abort their tasks."""
         dead_executors = await self._list_dead_executors()
         if dead_executors:
@@ -547,37 +589,61 @@
         """List executors with expired lifetime."""
         executors = await self._redis.hgetall(self.executor_map_key)
         t = time()
         dt = Limit.PING_INTERVAL.value * 4
         dead_executors = [key.decode('utf-8') for key, t0 in executors.items() if t - int(t0.decode('utf-8')) > dt]
         return dead_executors
 
+    async def _queue_timers(self):
+        """Queue tasks waiting for timers."""
+        sql = (
+            self.table.update()
+            .where(
+                sa.and_(
+                    self.table.c.wait_deadline < int(time()),
+                    self.table.c.status == TaskStatus.WAITING.value,
+                    self.table.c.enabled.is_(True),
+                )
+            )
+            .values(
+                {
+                    'status': TaskStatus.SUSPENDED.value,
+                    'result': self.table.c.result + [None],
+                    'stage': self.table.c.stage + 1,
+                    'wait_deadline': None,
+                    'executor_id': None,
+                }
+            )
+        )
+        await self._db.execute(sql)
+
     async def _queue_suspended_and_idle(self):
         """Queue all suspended tasks."""
         sql = (
             self.table.update()
             .where(
                 sa.or_(
                     sa.and_(
-                        self.table.c.status == TaskStatus.IDLE.value,
                         self.table.c.next_run < int(time()),
+                        self.table.c.status == TaskStatus.IDLE.value,
                         self.table.c.enabled.is_(True),
                     ),
                     sa.and_(
                         self.table.c.status == TaskStatus.SUSPENDED.value,
                         self.table.c.queued_at > int(time()) - self._suspended_lifetime * 3600,
                         self.table.c.enabled.is_(True),
                     ),
                 )
             )
             .values(
                 {
                     'status': TaskStatus.QUEUED.value,
                     'queued_at': int(time()),
                     'exec_deadline': int(time()) + self.table.c.max_exec_timeout,
+                    'wait_deadline': None,
                     'exit_code': None,
                     'error': None,
                 }
             )
             .returning(
                 self.table.c.id,
                 self.table.c.commands,
@@ -598,15 +664,17 @@
     async def _abort_timed_out_tasks(self):
         """Abort all queued tasks reached their timeout."""
         sql = (
             self.table.update()
             .where(
                 sa.and_(
                     self.table.c.queued_at < int(time()) - Limit.MIN_T.value - self.table.c.max_exec_timeout,
-                    self.table.c.status.in_([TaskStatus.QUEUED.value, TaskStatus.EXECUTED.value]),
+                    self.table.c.status.in_(
+                        [TaskStatus.QUEUED.value, TaskStatus.EXECUTED.value, TaskStatus.WAITING.value]
+                    ),
                     self.table.c.enabled.is_(True),
                 )
             )
             .values(
                 {
                     'status': TaskStatus.FAILED.value,
                     'error': None,
@@ -631,14 +699,15 @@
                 )
             )
             .values(
                 {
                     'status': TaskStatus.QUEUED.value,
                     'queued_at': int(time()),
                     'exec_deadline': int(time()) + self.table.c.max_exec_timeout,
+                    'wait_deadline': None,
                     'stage': sa.text(
                         f"CASE WHEN {self.table.c.restart_policy.name} = '{RestartPolicy.CURRENT.value}'"
                         f' THEN {self.table.c.stage.name}'
                         ' ELSE 0 END'
                     ),  # CURRENT or FIRST
                     'executor_id': None,
                     'retries': self.table.c.retries + 1,
@@ -683,14 +752,15 @@
             .values(
                 {
                     'status': TaskStatus.IDLE.value,
                     'result': [],
                     'stage': 0,
                     'executor_id': None,
                     'retries': 0,
+                    'wait_deadline': None
                     # 'exit_code': None,
                     # 'error': None,
                 }
             )
             .returning(self.table.c.id, self.table.c.cron)
         )
         async with self._db.begin() as conn:
@@ -748,26 +818,29 @@
         self,
         app,
         stream_client: StreamRPCClient = None,
         manager_app: str = None,
         manager_topic: str = Topic.MANAGER,
         rpc_service: JSONRPCServer = None,
         scheduler: Scheduler = None,
+        data: dict = None,
         logger=None,
     ):
         """Initialize.
 
         :param app: web app
         :param manager_app:
         :param manager_topic:
         :param rpc_service: local rpc server name or instance
         :param stream_client: stream client to the manager
+        :param data: additional data for command templates
         :param logger: optional logger instance
         """
         ContextableService.__init__(self, app=app, logger=logger)
+        self.data = data if data else {}
         self._rpc = rpc_service
         self._scheduler = scheduler
         self._manager_app = manager_app if manager_topic else self.app.name
         self._manager_topic = manager_topic
         self._stream = stream_client
         self._task_ping = None
         self._closing = True
@@ -800,26 +873,37 @@
         return self._closing
 
     async def run_task(self, data: ExecutorTask) -> None:
         """Run a task and callback its result to the manager."""
         stage, deadline = data['stage'], data['exec_deadline']
         self.logger.info('Acquired task', task_id=data['id'], stage=stage, deadline=deadline)
         template_data = self._create_template_dict(data)
-        headers = {
-            JSONRPCHeaders.REQUEST_DEADLINE_HEADER: deadline,
-            JSONRPCHeaders.CORRELATION_ID_HEADER: data['job_id'],
-        }
         for n, cmd in enumerate(data['commands']):
             if self._closing:
                 break
+
             stage = data['stage'] + n
-            await self._alert_on_stage_execution(data, stage)
             self.logger.info(
                 'Stage executed', task_id=data['id'], stage=stage, method=cmd['method'], deadline=data['exec_deadline']
             )
+            if cmd['method'] == Message.method:
+                return await self._wait_for_message(data, stage)
+            elif cmd['method'] == Timer.method:
+                return await self._wait_for_timer(data, stage, cmd['params']['timer'])
+
+            await self._alert_on_stage_execution(data, stage)
+            stage_timeout = cmd.get('max_timeout')
+            headers = {
+                JSONRPCHeaders.CORRELATION_ID_HEADER: data['job_id'],
+            }
+            if stage_timeout:
+                stage_deadline = int(time() + stage_timeout)
+                headers[JSONRPCHeaders.REQUEST_DEADLINE_HEADER] = min(stage_deadline, deadline)
+            else:
+                headers[JSONRPCHeaders.REQUEST_DEADLINE_HEADER] = deadline
             try:
                 cmd = Template(cmd).fill(template_data)
                 _, result = await self._rpc.call(body=cmd, headers=headers, scope=Scope.SYSTEM)
             except Exception as exc:
                 error = result = RPCError(
                     id=None, error=InternalError(base_exc=exc, message='Template evaluation error')
                 )
@@ -828,23 +912,22 @@
 
             if error:
                 self.logger.error(
                     'Stage failed', task_id=data['id'], stage=stage, method=cmd['method'], error=error['error']
                 )
                 await self._write_stage_result(data, stage, error=True, result=result)
                 return
-            else:
-                self.logger.info('Stage finished', task_id=data['id'], stage=stage, method=cmd['method'])
-                template_data[str(stage)] = result
-                await self._write_stage_result(data, stage, error=False, result=result)
 
-    @staticmethod
-    def _create_template_dict(data: ExecutorTask) -> dict:
+            self.logger.info('Stage finished', task_id=data['id'], stage=stage, method=cmd['method'])
+            template_data[str(stage)] = result
+            await self._write_stage_result(data, stage, error=False, result=result)
+
+    def _create_template_dict(self, data: ExecutorTask) -> dict:
         env = {str(stage): data['result'][stage] for stage in range(data['stage'])}
-        env['kws'] = data['kws']
+        env.update({'id': data['id'], 'kws': data['kws'], 'executor': self.data})
         return env
 
     @staticmethod
     def _parse_result(result) -> tuple:
         """Get error flag and result from rpc server response."""
         if isinstance(result, list):
             _result = []
@@ -855,78 +938,67 @@
                     result.append(r['result'])
             return False, _result
         elif 'error' in result:
             return result, result
         else:
             return False, result['result']
 
-    async def _alert_on_stage_execution(self, data: ExecutorTask, stage: int):
-        """Alert the manager on task execution."""
+    async def _call_manager(self, method: str, params: dict, job_id: str | None):
+        """Call the manager stream."""
+        headers = {}
+        if job_id:
+            headers[JSONRPCHeaders.CORRELATION_ID_HEADER] = job_id
         await retry(
             self._stream.call,
             kws=dict(
-                headers={JSONRPCHeaders.CORRELATION_ID_HEADER: data['job_id']},
-                method=f'{self.manager_service_name}.execute_stage',
-                params={'task_id': data['id'], 'executor_id': self.app.id, 'stage': stage},
+                headers=headers,
+                method=f'{self.manager_service_name}.{method}',
+                params=params,
                 app=self._manager_app,
                 topic=self._manager_topic,
             ),
-            retries=3,
+            retries=5,
             retry_timeout=1,
             logger=self.logger,
         )
 
-    async def _write_stage_result(self, data: ExecutorTask, stage: int, error: bool, result):
+    async def _wait_for_timer(self, data: ExecutorTask, stage: int, timer: int) -> None:
+        """Wait for a timer."""
+        params = {'task_id': data['id'], 'executor_id': self.app.id, 'stage': stage, 'deadline': int(time()) + timer}
+        await self._call_manager('wait_for_timer', params, data['job_id'])
+
+    async def _wait_for_message(self, data: ExecutorTask, stage: int) -> None:
+        """Wait until the task receives a callback message."""
+        params = {'task_id': data['id'], 'executor_id': self.app.id, 'stage': stage}
+        await self._call_manager('wait_for_message', params, data['job_id'])
+
+    async def _alert_on_stage_execution(self, data: ExecutorTask, stage: int) -> None:
+        """Alert the manager on task execution."""
+        params = {'task_id': data['id'], 'executor_id': self.app.id, 'stage': stage}
+        await self._call_manager('execute_stage', params, data['job_id'])
+
+    async def _write_stage_result(self, data: ExecutorTask, stage: int, error: bool, result) -> None:
         """Send task stage results to the manager."""
-        await retry(
-            self._stream.call,
-            kws=dict(
-                headers={JSONRPCHeaders.CORRELATION_ID_HEADER: data['job_id']},
-                method=f'{self.manager_service_name}.write_stage',
-                params={
-                    'task_id': data['id'],
-                    'executor_id': self.app.id,
-                    'stage': stage,
-                    'stages': data['stages'],
-                    'result': result,
-                    'error': error,
-                },
-                app=self._manager_app,
-                topic=self._manager_topic,
-            ),
-            retries=3,
-            retry_timeout=1,
-            logger=self.logger,
-        )
+        params = {
+            'task_id': data['id'],
+            'executor_id': self.app.id,
+            'stage': stage,
+            'stages': data['stages'],
+            'result': result,
+            'error': error,
+        }
+        await self._call_manager('write_stage', params, data['job_id'])
 
-    async def _send_ping(self):
+    async def _send_ping(self) -> None:
         """Send a health report message to the manager."""
-        if self._closing:
-            return
-        await self._stream.call(
-            method=f'{self.manager_service_name}.ping',
-            params={'executor_id': self.app.id},
-            app=self._manager_app,
-            topic=self._manager_topic,
-        )
+        if not self._closing:
+            await self._call_manager('ping', {'executor_id': self.app.id}, None)
 
-    async def _suspend_self(self):
+    async def _suspend_self(self) -> None:
         """Send an executor suspend message to the manager."""
-        self.logger.info('Suspending executor')
-        await retry(
-            self._stream.call,
-            kws=dict(
-                method=f'{self.manager_service_name}.suspend_executor',
-                params={'executor_id': self.app.id},
-                app=self._manager_app,
-                topic=self._manager_topic,
-            ),
-            retries=3,
-            retry_timeout=1,
-            logger=self.logger,
-        )
+        await self._call_manager('suspend_executor', {'executor_id': self.app.id}, None)
 
 
 SERVICE_CLASS_REGISTRY.register(TaskService)
 SERVICE_CLASS_REGISTRY.register(NotificationService)
 SERVICE_CLASS_REGISTRY.register(TaskManager)
 SERVICE_CLASS_REGISTRY.register(TaskExecutor)
```

## kaiju_tasks/types.py

```diff
@@ -1,24 +1,94 @@
 """Data types."""
-
-from enum import Enum
+import abc
+from dataclasses import dataclass
 from datetime import datetime
-from typing import Optional, TypedDict, List, Union
+from enum import Enum
+from typing import ClassVar, List, Optional, Tuple, Type, TypedDict, Union
 from uuid import UUID
 
+from kaiju_tools.encoding import Serializable
+from kaiju_tools.registry import ClassRegistry
 from kaiju_tools.rpc import RPCRequest
 
-__all__ = ['TaskStatus', 'RestartPolicy', 'Limit', 'TaskCommand', 'Task', 'Notification', 'ExecutorTask']
+
+__all__ = [
+    'TaskStatus',
+    'RestartPolicy',
+    'Limit',
+    'TaskCommand',
+    'Task',
+    'Notification',
+    'ExecutorTask',
+    'Message',
+    'Timer',
+    'SpecialCommandsRegistry',
+    'SPECIAL_COMMANDS',
+]
 
 
 class TaskCommand(TypedDict, total=False):
     """Task command (similar to RPC request)."""
 
     method: str
     params: Optional[dict]
+    max_timeout: Optional[int]
+
+
+class _SpecialCommand(Serializable, abc.ABC):
+    """Special instructions for the executor."""
+
+    method: ClassVar[str]
+
+    @abc.abstractmethod
+    def repr(self) -> TaskCommand:
+        """Get a task command dict."""
+
+
+@dataclass(slots=True)
+class Message(_SpecialCommand):
+    """Message hook.
+
+    The task must wait until a message is received for this particular task to continue.
+    """
+
+    method = '_MESSAGE_'
+    max_timeout: Optional[int] = None
+
+    def repr(self) -> TaskCommand:
+        return TaskCommand(method=self.method, params=None, max_timeout=self.max_timeout)
+
+
+class SpecialCommandsRegistry(ClassRegistry[str, _SpecialCommand]):
+    """Registry of special task commands."""
+
+    @classmethod
+    def get_base_classes(cls) -> Tuple[Type, ...]:
+        return (_SpecialCommand,)
+
+    def get_key(self, obj: _SpecialCommand) -> str:
+        return obj.method
+
+
+SPECIAL_COMMANDS = SpecialCommandsRegistry()
+SPECIAL_COMMANDS.register_from_namespace(locals())
+
+
+@dataclass(slots=True)
+class Timer(_SpecialCommand):
+    """Timer hook.
+
+    The task must wait for a timer and continue.
+    """
+
+    method = '_TIMER_'
+    timer: int
+
+    def repr(self) -> TaskCommand:
+        return TaskCommand(method=self.method, params={'timer': self.timer})
 
 
 class Limit(Enum):
     """Parameter limits and settings."""
 
     MAX_STAGES = 100  #: max number of stages per task
     MAX_RETRIES = 10  #: max retries per job
@@ -33,14 +103,15 @@
 
     IDLE = 'IDLE'  #: initialized in the table
     QUEUED = 'QUEUED'  #: sent to an executor stream
     EXECUTED = 'EXECUTED'  #: accepted by an executor
     FINISHED = 'FINISHED'  #: all stages completed
     FAILED = 'FAILED'  #: error during stage execution
     SUSPENDED = 'SUSPENDED'  #: executor suspended, waiting for re-queuing
+    WAITING = 'WAITING'  #: task is waiting for external data to finish
 
 
 class RestartPolicy(Enum):
     """Task restart policy types."""
 
     CURRENT = 'CURRENT'  #: restart from the current stage
     FIRST = 'FIRST'  #: restart from the first stage
@@ -77,14 +148,15 @@
 
     status: str  #: current task status
     result: list  #: task execution result, a list of stage returns
     stage: int  #: current stage being executed (or about to execute)
     stages: int  #: total number of stages
     queued_at: Optional[int]  #: UNIX time last queued
     exec_deadline: Optional[int]  #: UNIX time deadline
+    wait_deadline: Optional[int]  #: UNIX time deadline for a timer command (see `Timer`)
     next_run: Optional[int]  #: UNIX time for next run
     user_id: Optional[UUID]  #: user created the task
     executor_id: Optional[UUID]  #: which executor has this task
     job_id: Optional[str]  #: updated for each new run
     retries: int  #: current number of retries
     created: datetime  #: when task record was added to the table
     exit_code: Optional[int]  #: exit (error) code similar to UNIX codes
```

## kaiju_tasks/tests/test_tasks.py

```diff
@@ -5,15 +5,15 @@
 from uuid import uuid4
 
 import pytest  # noqa: pycharm
 import pytest_asyncio
 
 from kaiju_db.tests.test_db import TestSQLService
 
-from kaiju_tasks.types import Task, Notification, TaskStatus, ExecutorTask, TaskCommand, RestartPolicy
+from kaiju_tasks.types import Task, Notification, TaskStatus, ExecutorTask, TaskCommand, RestartPolicy, Timer, Message
 from kaiju_tasks.services import TaskService, NotificationService, TaskExecutor
 from kaiju_tasks.gui import TaskGUI
 
 __all__ = ['TestTaskService', 'TestNotificationService', 'TestTaskExecutor', 'TestTaskManager', 'TaskGUI']
 
 
 @pytest.mark.asyncio
@@ -35,14 +35,25 @@
                 commands=[
                     {'method': 'do.echo', 'params': {'data': '[kws.data]'}},
                     {'method': 'do.echo', 'params': {'data': '[0.result]'}},
                 ],
                 kws={'data': n},
             )
 
+    async def test_write_message(self, _store, _row):
+        _store = cast(TaskService, _store)
+        _row = await _store.create(_row)
+        _store._validator = lambda o: o
+        await _store.update(_row['id'], Task(status=TaskStatus.WAITING.value))
+        await _store.write_message(_row['id'], {'test': True})
+        task = await _store.get(_row['id'])
+        assert task['status'] == TaskStatus.SUSPENDED.value
+        assert task['result'] == [{'test': True}]
+        assert task['stage'] == 1
+
     async def test_task_reset(self, _store, _row):
         _store = cast(TaskService, _store)
         _row = await _store.create(_row)
         _store._validator = lambda o: o
         await _store.update(_row['id'], Task(status=TaskStatus.EXECUTED.value, job_id='job', stage=1))  # running task
         await _store.reset_task(_row['id'])
         task = await _store.get(_row['id'])
@@ -93,14 +104,56 @@
 
     async def test_executor_suspend(self, _service: TaskExecutor, mock_stream_client):
         await _service._suspend_self()
         stream = next(iter(mock_stream_client._transport._stream.values()))
         reqs = [stream.get_nowait()[0][0] for _ in range(stream.qsize())]
         assert 'taskman.suspend_executor' in reqs
 
+    async def test_task_timers(self, _service: TaskExecutor, mock_stream_client):
+        task = ExecutorTask(
+            id=uuid4().hex,
+            commands=[
+                TaskCommand(method='do.echo', params={'data': True}),
+                Timer(100).repr(),
+                TaskCommand(method='do.echo', params={'data': False}),
+            ],
+            kws={},
+            result=[],
+            stage=0,
+            stages=3,
+            exec_deadline=int(time() + 1000),
+            job_id='123',
+        )
+        await _service.run_task(task)
+        stream = next(iter(mock_stream_client._transport._stream.values()))
+        reqs = [stream.get_nowait()[0] for _ in range(stream.qsize())]
+        methods = [r[0] for r in reqs if r[0] != 'taskman.ping']
+        assert methods == ['taskman.execute_stage', 'taskman.write_stage', 'taskman.wait_for_timer']
+
+    async def test_task_messages(self, _service: TaskExecutor, mock_stream_client):
+        task = ExecutorTask(
+            id=uuid4().hex,
+            commands=[
+                TaskCommand(method='do.echo', params={'data': True}),
+                Message().repr(),
+                TaskCommand(method='do.echo', params={'data': False}),
+            ],
+            kws={},
+            result=[],
+            stage=0,
+            stages=3,
+            exec_deadline=int(time() + 1000),
+            job_id='123',
+        )
+        await _service.run_task(task)
+        stream = next(iter(mock_stream_client._transport._stream.values()))
+        reqs = [stream.get_nowait()[0] for _ in range(stream.qsize())]
+        methods = [r[0] for r in reqs if r[0] != 'taskman.ping']
+        assert methods == ['taskman.execute_stage', 'taskman.write_stage', 'taskman.wait_for_message']
+
     async def test_task_execution(self, _service: TaskExecutor, mock_stream_client):
         value_1, value_2 = uuid4(), uuid4()
         task = ExecutorTask(
             id=uuid4().hex,
             commands=[
                 TaskCommand(method='do.echo', params={'data': value_1}),
                 TaskCommand(method='do.echo', params={'data': '[kws.value_2]'}),
@@ -201,14 +254,22 @@
                 {'status': TaskStatus.IDLE.value},
             ),
             ({'status': TaskStatus.FINISHED.value}, {'status': TaskStatus.FINISHED.value}),
             (
                 {'status': TaskStatus.FINISHED.value, 'cron': '* * * * 5', 'stage': 1, 'retries': 3, 'result': [1, 2]},
                 {'status': TaskStatus.IDLE.value, 'stage': 0, 'retries': 0, 'result': []},
             ),
+            (
+                {'status': TaskStatus.WAITING.value, 'queued_at': int(time()), 'wait_deadline': int(time()) - 1},
+                {'status': TaskStatus.QUEUED.value},
+            ),
+            (
+                {'status': TaskStatus.WAITING.value, 'queued_at': int(time())},
+                {'status': TaskStatus.WAITING.value},
+            ),
         ],
         ids=[
             'IDLE',
             'IDLE not ready',
             'IDLE inactive',
             'QUEUED timeout',
             'SUSPENDED',
@@ -217,14 +278,16 @@
             'FAILED with restart',
             'FAILED with restart from stage 0',
             'FAILED inactive',
             'FAILED no restarts left',
             'FAILED cron',
             'FINISHED',
             'FINISHED cron',
+            'WAITING timer',
+            'WAITING message',
         ],
     )
     async def test_task_management(self, _service, task_service, before_queue, after_queue):
         task_service._validator = lambda o: o
         task = await task_service.create({'commands': [{'method': 'do'}, {'method': 'do.2'}]}, columns=['id'])
         task = await task_service.update(task['id'], before_queue, columns='*')
         await asyncio.sleep(1)
```

## Comparing `kaiju_tasks-2.1.6.dist-info/LICENSE` & `kaiju_tasks-2.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_tasks-2.1.6.dist-info/METADATA` & `kaiju_tasks-2.1.7.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 Metadata-Version: 2.1
 Name: kaiju-tasks
-Version: 2.1.6
+Version: 2.1.7
 Summary: Service and user task management
 Home-page: https://gitlab.com/kaiju-python/kaiju-tasks
 Author: antonnidhoggr@me.com
 Author-email: antonnidhoggr@me.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: croniter (>=1.4.1)
 Requires-Dist: kaiju-tools (<3,>=2)
 Requires-Dist: kaiju-db (<3,>=2)
 Requires-Dist: kaiju-redis (<3,>=2)
 Requires-Dist: kaiju-model (<3,>=2)
 Provides-Extra: dev
 Requires-Dist: bump2version (>=1.0) ; extra == 'dev'
 Requires-Dist: pyroma (>=4.1) ; extra == 'dev'
 Requires-Dist: bandit (>=1.7) ; extra == 'dev'
 Requires-Dist: black (>=22.12) ; extra == 'dev'
 Requires-Dist: flake8 (>=6.0) ; extra == 'dev'
 Requires-Dist: pyproject-flake8 ; extra == 'dev'
+Requires-Dist: flake8-walrus (>=1.2.0) ; extra == 'dev'
 Requires-Dist: pre-commit (>=3.1) ; extra == 'dev'
 Requires-Dist: pydocstyle (>=6.2) ; extra == 'dev'
 Requires-Dist: setup-cfg-fmt (>=2.2) ; extra == 'dev'
 Requires-Dist: restructuredtext-lint (>=1.4) ; extra == 'dev'
 Requires-Dist: tox (>=3.28) ; extra == 'dev'
 Requires-Dist: tox-pyenv (>=1.1) ; extra == 'dev'
 Requires-Dist: pip-tools (>=6.13) ; extra == 'dev'
 Requires-Dist: towncrier (>=23.6) ; extra == 'dev'
 Requires-Dist: pyupgrade (>=3.4) ; extra == 'dev'
+Requires-Dist: isort (>=5.12.0) ; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: sphinx ; extra == 'docs'
 Requires-Dist: python-docs-theme ; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pytest (>=7.4) ; extra == 'test'
 Requires-Dist: pytest-asyncio (>=0.21) ; extra == 'test'
 Requires-Dist: docker (>=6.1.3) ; extra == 'test'
```

