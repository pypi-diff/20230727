# Comparing `tmp/netbluemind4-4.9.2928.tar.gz` & `tmp/netbluemind4-4.9.2940.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbluemind4-4.9.2928.tar", last modified: Wed Jul 19 06:59:15 2023, max compression
+gzip compressed data, was "netbluemind4-4.9.2940.tar", last modified: Thu Jul 27 13:48:42 2023, max compression
```

## Comparing `netbluemind4-4.9.2928.tar` & `netbluemind4-4.9.2940.tar`

### file list

```diff
@@ -1,638 +1,638 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.371159 netbluemind4-4.9.2928/
--rw-r--r--   0 root         (0) root         (0)     2232 2023-07-19 06:58:14.000000 netbluemind4-4.9.2928/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      534 2023-07-19 06:59:15.375159 netbluemind4-4.9.2928/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      461 2023-07-19 06:58:14.000000 netbluemind4-4.9.2928/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.243156 netbluemind4-4.9.2928/netbluemind/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:10.000000 netbluemind4-4.9.2928/netbluemind/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.243156 netbluemind4-4.9.2928/netbluemind/addressbook/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:02.000000 netbluemind4-4.9.2928/netbluemind/addressbook/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.255156 netbluemind4-4.9.2928/netbluemind/addressbook/api/
--rw-r--r--   0 root         (0) root         (0)     3021 2023-07-19 06:59:06.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/AddressBookDescriptor.py
--rw-r--r--   0 root         (0) root         (0)    24796 2023-07-19 06:59:05.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/IAddressBook.py
--rw-r--r--   0 root         (0) root         (0)     3064 2023-07-19 06:59:06.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/IAddressBookUids.py
--rw-r--r--   0 root         (0) root         (0)     2156 2023-07-19 06:59:03.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/IAddressBooks.py
--rw-r--r--   0 root         (0) root         (0)     7034 2023-07-19 06:59:03.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/IAddressBooksMgmt.py
--rw-r--r--   0 root         (0) root         (0)     2734 2023-07-19 06:59:03.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/IVCardService.py
--rw-r--r--   0 root         (0) root         (0)     6805 2023-07-19 06:59:05.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCard.py
--rw-r--r--   0 root         (0) root         (0)     2204 2023-07-19 06:59:04.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardBasicAttribute.py
--rw-r--r--   0 root         (0) root         (0)     3405 2023-07-19 06:59:03.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardChanges.py
--rw-r--r--   0 root         (0) root         (0)     2218 2023-07-19 06:59:02.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardChangesItemAdd.py
--rw-r--r--   0 root         (0) root         (0)     1515 2023-07-19 06:59:03.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardChangesItemDelete.py
--rw-r--r--   0 root         (0) root         (0)     2227 2023-07-19 06:59:03.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardChangesItemModify.py
--rw-r--r--   0 root         (0) root         (0)     4211 2023-07-19 06:59:03.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardCommunications.py
--rw-r--r--   0 root         (0) root         (0)     1705 2023-07-19 06:59:03.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardCommunicationsEmail.py
--rw-r--r--   0 root         (0) root         (0)     1702 2023-07-19 06:59:04.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardCommunicationsImpp.py
--rw-r--r--   0 root         (0) root         (0)     1702 2023-07-19 06:59:04.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardCommunicationsLang.py
--rw-r--r--   0 root         (0) root         (0)     1894 2023-07-19 06:59:04.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardCommunicationsTel.py
--rw-r--r--   0 root         (0) root         (0)     2085 2023-07-19 06:59:03.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardDeliveryAddressing.py
--rw-r--r--   0 root         (0) root         (0)     3596 2023-07-19 06:59:06.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardDeliveryAddressingAddress.py
--rw-r--r--   0 root         (0) root         (0)     2750 2023-07-19 06:59:03.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardExplanatory.py
--rw-r--r--   0 root         (0) root         (0)     1690 2023-07-19 06:59:05.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardExplanatoryUrl.py
--rw-r--r--   0 root         (0) root         (0)     5236 2023-07-19 06:59:06.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardIdentification.py
--rw-r--r--   0 root         (0) root         (0)     1726 2023-07-19 06:59:03.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardIdentificationFormatedName.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-07-19 06:59:06.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardIdentificationGender.py
--rw-r--r--   0 root         (0) root         (0)     3023 2023-07-19 06:59:05.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardIdentificationName.py
--rw-r--r--   0 root         (0) root         (0)     1714 2023-07-19 06:59:03.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardIdentificationNickname.py
--rw-r--r--   0 root         (0) root         (0)     3734 2023-07-19 06:59:05.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardInfo.py
--rw-r--r--   0 root         (0) root         (0)     1140 2023-07-19 06:59:03.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardKind.py
--rw-r--r--   0 root         (0) root         (0)     3115 2023-07-19 06:59:04.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardOrganizational.py
--rw-r--r--   0 root         (0) root         (0)     2316 2023-07-19 06:59:05.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardOrganizationalMember.py
--rw-r--r--   0 root         (0) root         (0)     2049 2023-07-19 06:59:06.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardOrganizationalOrg.py
--rw-r--r--   0 root         (0) root         (0)     1722 2023-07-19 06:59:05.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardParameter.py
--rw-r--r--   0 root         (0) root         (0)     2788 2023-07-19 06:59:04.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardQuery.py
--rw-r--r--   0 root         (0) root         (0)     1136 2023-07-19 06:59:03.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardQueryOrderBy.py
--rw-r--r--   0 root         (0) root         (0)     1992 2023-07-19 06:59:06.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardRelated.py
--rw-r--r--   0 root         (0) root         (0)     1866 2023-07-19 06:59:03.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardSecurity.py
--rw-r--r--   0 root         (0) root         (0)     1681 2023-07-19 06:59:05.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardSecurityKey.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:02.000000 netbluemind4-4.9.2928/netbluemind/addressbook/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.255156 netbluemind4-4.9.2928/netbluemind/attachment/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:10.000000 netbluemind4-4.9.2928/netbluemind/attachment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.255156 netbluemind4-4.9.2928/netbluemind/attachment/api/
--rw-r--r--   0 root         (0) root         (0)     2228 2023-07-19 06:58:25.000000 netbluemind4-4.9.2928/netbluemind/attachment/api/AttachedFile.py
--rw-r--r--   0 root         (0) root         (0)     2196 2023-07-19 06:58:25.000000 netbluemind4-4.9.2928/netbluemind/attachment/api/Configuration.py
--rw-r--r--   0 root         (0) root         (0)     3699 2023-07-19 06:58:25.000000 netbluemind4-4.9.2928/netbluemind/attachment/api/IAttachment.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:10.000000 netbluemind4-4.9.2928/netbluemind/attachment/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.255156 netbluemind4-4.9.2928/netbluemind/authentication/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:04.000000 netbluemind4-4.9.2928/netbluemind/authentication/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.259157 netbluemind4-4.9.2928/netbluemind/authentication/api/
--rw-r--r--   0 root         (0) root         (0)     2214 2023-07-19 06:59:09.000000 netbluemind4-4.9.2928/netbluemind/authentication/api/APIKey.py
--rw-r--r--   0 root         (0) root         (0)     4622 2023-07-19 06:59:08.000000 netbluemind4-4.9.2928/netbluemind/authentication/api/AccessTokenInfo.py
--rw-r--r--   0 root         (0) root         (0)     1205 2023-07-19 06:59:07.000000 netbluemind4-4.9.2928/netbluemind/authentication/api/AccessTokenInfoTokenStatus.py
--rw-r--r--   0 root         (0) root         (0)     3330 2023-07-19 06:59:08.000000 netbluemind4-4.9.2928/netbluemind/authentication/api/AuthUser.py
--rw-r--r--   0 root         (0) root         (0)     3891 2023-07-19 06:59:08.000000 netbluemind4-4.9.2928/netbluemind/authentication/api/IAPIKeys.py
--rw-r--r--   0 root         (0) root         (0)     6122 2023-07-19 06:59:09.000000 netbluemind4-4.9.2928/netbluemind/authentication/api/IAuthentication.py
--rw-r--r--   0 root         (0) root         (0)     2400 2023-07-19 06:59:08.000000 netbluemind4-4.9.2928/netbluemind/authentication/api/ISecurityToken.py
--rw-r--r--   0 root         (0) root         (0)     1387 2023-07-19 06:59:08.000000 netbluemind4-4.9.2928/netbluemind/authentication/api/ISudoSupport.py
--rw-r--r--   0 root         (0) root         (0)     2334 2023-07-19 06:59:08.000000 netbluemind4-4.9.2928/netbluemind/authentication/api/IUserAccessToken.py
--rw-r--r--   0 root         (0) root         (0)     3151 2023-07-19 06:59:08.000000 netbluemind4-4.9.2928/netbluemind/authentication/api/LoginResponse.py
--rw-r--r--   0 root         (0) root         (0)     1132 2023-07-19 06:59:08.000000 netbluemind4-4.9.2928/netbluemind/authentication/api/LoginResponseStatus.py
--rw-r--r--   0 root         (0) root         (0)     1167 2023-07-19 06:59:08.000000 netbluemind4-4.9.2928/netbluemind/authentication/api/ValidationKind.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:04.000000 netbluemind4-4.9.2928/netbluemind/authentication/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.259157 netbluemind4-4.9.2928/netbluemind/backend/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:04.000000 netbluemind4-4.9.2928/netbluemind/backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.259157 netbluemind4-4.9.2928/netbluemind/backend/mail/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:04.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.267157 netbluemind4-4.9.2928/netbluemind/backend/mail/api/
--rw-r--r--   0 root         (0) root         (0)     2063 2023-07-19 06:58:32.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/Conversation.py
--rw-r--r--   0 root         (0) root         (0)     1987 2023-07-19 06:58:33.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/ConversationMessageRef.py
--rw-r--r--   0 root         (0) root         (0)     1118 2023-07-19 06:58:33.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/DispositionType.py
--rw-r--r--   0 root         (0) root         (0)    10560 2023-07-19 06:58:37.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/IBaseMailboxFolders.py
--rw-r--r--   0 root         (0) root         (0)     2769 2023-07-19 06:58:32.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/IItemsTransfer.py
--rw-r--r--   0 root         (0) root         (0)     4309 2023-07-19 06:58:38.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/IMailConversation.py
--rw-r--r--   0 root         (0) root         (0)     6827 2023-07-19 06:58:33.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/IMailConversationActions.py
--rw-r--r--   0 root         (0) root         (0)    19004 2023-07-19 06:58:35.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/IMailboxFolders.py
--rw-r--r--   0 root         (0) root         (0)    19154 2023-07-19 06:58:33.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/IMailboxFoldersByContainer.py
--rw-r--r--   0 root         (0) root         (0)    21454 2023-07-19 06:58:37.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/IMailboxItems.py
--rw-r--r--   0 root         (0) root         (0)     1731 2023-07-19 06:58:35.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/IOutbox.py
--rw-r--r--   0 root         (0) root         (0)    10771 2023-07-19 06:58:38.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/IReadOnlyMailboxFolders.py
--rw-r--r--   0 root         (0) root         (0)     1579 2023-07-19 06:58:31.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/IUserInbox.py
--rw-r--r--   0 root         (0) root         (0)     1759 2023-07-19 06:58:37.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/ImapAck.py
--rw-r--r--   0 root         (0) root         (0)     1884 2023-07-19 06:58:32.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/ImapItemIdentifier.py
--rw-r--r--   0 root         (0) root         (0)     3634 2023-07-19 06:58:32.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/ImportMailboxItemSet.py
--rw-r--r--   0 root         (0) root         (0)     1535 2023-07-19 06:58:38.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/ImportMailboxItemSetMailboxItemId.py
--rw-r--r--   0 root         (0) root         (0)     3090 2023-07-19 06:58:35.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/ImportMailboxItemsStatus.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-07-19 06:58:35.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/ImportMailboxItemsStatusImportStatus.py
--rw-r--r--   0 root         (0) root         (0)     1864 2023-07-19 06:58:38.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/ImportMailboxItemsStatusImportedMailboxItem.py
--rw-r--r--   0 root         (0) root         (0)     2219 2023-07-19 06:58:37.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/MailboxFolder.py
--rw-r--r--   0 root         (0) root         (0)     2397 2023-07-19 06:58:37.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/MailboxFolderSearchQuery.py
--rw-r--r--   0 root         (0) root         (0)     2723 2023-07-19 06:58:31.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/MailboxItem.py
--rw-r--r--   0 root         (0) root         (0)     5517 2023-07-19 06:58:34.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/MessageBody.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-07-19 06:58:31.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/MessageBodyHeader.py
--rw-r--r--   0 root         (0) root         (0)     4943 2023-07-19 06:58:35.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/MessageBodyPart.py
--rw-r--r--   0 root         (0) root         (0)     2397 2023-07-19 06:58:35.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/MessageBodyRecipient.py
--rw-r--r--   0 root         (0) root         (0)     1239 2023-07-19 06:58:38.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/MessageBodyRecipientKind.py
--rw-r--r--   0 root         (0) root         (0)     4966 2023-07-19 06:58:38.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/MessageSearchResult.py
--rw-r--r--   0 root         (0) root         (0)     2088 2023-07-19 06:58:34.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/MessageSearchResultMbox.py
--rw-r--r--   0 root         (0) root         (0)     5250 2023-07-19 06:58:33.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/SearchQuery.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-07-19 06:58:33.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/SearchQueryFolderScope.py
--rw-r--r--   0 root         (0) root         (0)     1722 2023-07-19 06:58:35.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/SearchQueryHeader.py
--rw-r--r--   0 root         (0) root         (0)     2800 2023-07-19 06:58:35.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/SearchQueryHeaderQuery.py
--rw-r--r--   0 root         (0) root         (0)     1129 2023-07-19 06:58:32.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/SearchQueryLogicalOperator.py
--rw-r--r--   0 root         (0) root         (0)     2360 2023-07-19 06:58:37.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/SearchQuerySearchScope.py
--rw-r--r--   0 root         (0) root         (0)     2563 2023-07-19 06:58:33.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/SearchResult.py
--rw-r--r--   0 root         (0) root         (0)     2030 2023-07-19 06:58:33.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/SearchSort.py
--rw-r--r--   0 root         (0) root         (0)     1100 2023-07-19 06:58:33.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/SearchSortOrder.py
--rw-r--r--   0 root         (0) root         (0)     2118 2023-07-19 06:58:35.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/SearchSortSortCriteria.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:04.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.271157 netbluemind4-4.9.2928/netbluemind/backend/mail/api/flags/
--rw-r--r--   0 root         (0) root         (0)     2408 2023-07-19 06:58:39.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/flags/ConversationFlagUpdate.py
--rw-r--r--   0 root         (0) root         (0)     2274 2023-07-19 06:58:38.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/flags/FlagUpdate.py
--rw-r--r--   0 root         (0) root         (0)     2340 2023-07-19 06:58:38.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/flags/ImportMailboxConversationSet.py
--rw-r--r--   0 root         (0) root         (0)     1710 2023-07-19 06:58:39.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/flags/MailboxItemFlag.py
--rw-r--r--   0 root         (0) root         (0)     1196 2023-07-19 06:58:39.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/flags/MailboxItemFlagSystem.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:04.000000 netbluemind4-4.9.2928/netbluemind/backend/mail/api/flags/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.271157 netbluemind4-4.9.2928/netbluemind/calendar/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:04.000000 netbluemind4-4.9.2928/netbluemind/calendar/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.291157 netbluemind4-4.9.2928/netbluemind/calendar/api/
--rw-r--r--   0 root         (0) root         (0)     2788 2023-07-19 06:58:26.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/CalendarDescriptor.py
--rw-r--r--   0 root         (0) root         (0)     3116 2023-07-19 06:58:27.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/CalendarLookupResponse.py
--rw-r--r--   0 root         (0) root         (0)     1145 2023-07-19 06:58:27.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/CalendarLookupResponseType.py
--rw-r--r--   0 root         (0) root         (0)     3050 2023-07-19 06:58:28.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/CalendarSettingsData.py
--rw-r--r--   0 root         (0) root         (0)     1188 2023-07-19 06:58:26.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/CalendarSettingsDataDay.py
--rw-r--r--   0 root         (0) root         (0)     2770 2023-07-19 06:58:27.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/CalendarView.py
--rw-r--r--   0 root         (0) root         (0)     1177 2023-07-19 06:58:26.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/CalendarViewCalendarViewType.py
--rw-r--r--   0 root         (0) root         (0)     3600 2023-07-19 06:58:27.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/CalendarViewChanges.py
--rw-r--r--   0 root         (0) root         (0)     2066 2023-07-19 06:58:27.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/CalendarViewChangesItemAdd.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-07-19 06:58:27.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/CalendarViewChangesItemDelete.py
--rw-r--r--   0 root         (0) root         (0)     2075 2023-07-19 06:58:27.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/CalendarViewChangesItemModify.py
--rw-r--r--   0 root         (0) root         (0)     2436 2023-07-19 06:58:28.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/CalendarsVEventQuery.py
--rw-r--r--   0 root         (0) root         (0)    24195 2023-07-19 06:58:29.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/ICalendar.py
--rw-r--r--   0 root         (0) root         (0)     2750 2023-07-19 06:58:28.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/ICalendarAutocomplete.py
--rw-r--r--   0 root         (0) root         (0)     2440 2023-07-19 06:58:27.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/ICalendarSettings.py
--rw-r--r--   0 root         (0) root         (0)     2496 2023-07-19 06:58:31.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/ICalendarUids.py
--rw-r--r--   0 root         (0) root         (0)     6957 2023-07-19 06:58:30.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/ICalendarView.py
--rw-r--r--   0 root         (0) root         (0)     1467 2023-07-19 06:58:28.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/ICalendarViewUids.py
--rw-r--r--   0 root         (0) root         (0)     3049 2023-07-19 06:58:28.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/ICalendars.py
--rw-r--r--   0 root         (0) root         (0)     4943 2023-07-19 06:58:30.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/ICalendarsMgmt.py
--rw-r--r--   0 root         (0) root         (0)     3067 2023-07-19 06:58:31.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/IFreebusyMgmt.py
--rw-r--r--   0 root         (0) root         (0)     1448 2023-07-19 06:58:31.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/IFreebusyUids.py
--rw-r--r--   0 root         (0) root         (0)     1752 2023-07-19 06:58:30.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/IPrint.py
--rw-r--r--   0 root         (0) root         (0)     3473 2023-07-19 06:58:31.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/IPublicFreebusy.py
--rw-r--r--   0 root         (0) root         (0)     3665 2023-07-19 06:58:27.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/IPublishCalendar.py
--rw-r--r--   0 root         (0) root         (0)    14235 2023-07-19 06:58:26.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/IUserCalendarViews.py
--rw-r--r--   0 root         (0) root         (0)     2596 2023-07-19 06:58:27.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/IVEvent.py
--rw-r--r--   0 root         (0) root         (0)     2623 2023-07-19 06:58:31.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/IVFreebusy.py
--rw-r--r--   0 root         (0) root         (0)     1692 2023-07-19 06:58:30.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/PrintData.py
--rw-r--r--   0 root         (0) root         (0)     5946 2023-07-19 06:58:27.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/PrintOptions.py
--rw-r--r--   0 root         (0) root         (0)     1746 2023-07-19 06:58:28.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/PrintOptionsCalendarMetadata.py
--rw-r--r--   0 root         (0) root         (0)     1156 2023-07-19 06:58:27.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/PrintOptionsPrintFormat.py
--rw-r--r--   0 root         (0) root         (0)     1144 2023-07-19 06:58:27.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/PrintOptionsPrintLayout.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-07-19 06:58:26.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/PrintOptionsPrintView.py
--rw-r--r--   0 root         (0) root         (0)     1100 2023-07-19 06:58:31.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/PublishMode.py
--rw-r--r--   0 root         (0) root         (0)     2821 2023-07-19 06:58:27.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/VEvent.py
--rw-r--r--   0 root         (0) root         (0)     2695 2023-07-19 06:58:26.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/VEventAttendeeQuery.py
--rw-r--r--   0 root         (0) root         (0)     3402 2023-07-19 06:58:28.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/VEventChanges.py
--rw-r--r--   0 root         (0) root         (0)     2375 2023-07-19 06:58:31.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/VEventChangesItemAdd.py
--rw-r--r--   0 root         (0) root         (0)     1845 2023-07-19 06:58:27.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/VEventChangesItemDelete.py
--rw-r--r--   0 root         (0) root         (0)     2384 2023-07-19 06:58:30.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/VEventChangesItemModify.py
--rw-r--r--   0 root         (0) root         (0)     2667 2023-07-19 06:58:30.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/VEventCounter.py
--rw-r--r--   0 root         (0) root         (0)     1815 2023-07-19 06:58:27.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/VEventCounterCounterOriginator.py
--rw-r--r--   0 root         (0) root         (0)     2112 2023-07-19 06:58:27.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/VEventOccurrence.py
--rw-r--r--   0 root         (0) root         (0)     4230 2023-07-19 06:58:30.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/VEventQuery.py
--rw-r--r--   0 root         (0) root         (0)     3935 2023-07-19 06:58:28.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/VEventSeries.py
--rw-r--r--   0 root         (0) root         (0)     1129 2023-07-19 06:58:28.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/VEventTransparency.py
--rw-r--r--   0 root         (0) root         (0)     2958 2023-07-19 06:58:30.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/VFreebusy.py
--rw-r--r--   0 root         (0) root         (0)     2996 2023-07-19 06:58:26.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/VFreebusyQuery.py
--rw-r--r--   0 root         (0) root         (0)     3128 2023-07-19 06:58:28.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/VFreebusySlot.py
--rw-r--r--   0 root         (0) root         (0)     1172 2023-07-19 06:58:26.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/VFreebusyType.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:04.000000 netbluemind4-4.9.2928/netbluemind/calendar/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.291157 netbluemind4-4.9.2928/netbluemind/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:06.000000 netbluemind4-4.9.2928/netbluemind/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.291157 netbluemind4-4.9.2928/netbluemind/core/api/
--rw-r--r--   0 root         (0) root         (0)     2011 2023-07-19 06:58:47.000000 netbluemind4-4.9.2928/netbluemind/core/api/Email.py
--rw-r--r--   0 root         (0) root         (0)     1736 2023-07-19 06:58:47.000000 netbluemind4-4.9.2928/netbluemind/core/api/ImportStats.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-07-19 06:58:47.000000 netbluemind4-4.9.2928/netbluemind/core/api/ListResult.py
--rw-r--r--   0 root         (0) root         (0)     2211 2023-07-19 06:58:47.000000 netbluemind4-4.9.2928/netbluemind/core/api/VersionInfo.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:02.000000 netbluemind4-4.9.2928/netbluemind/core/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.291157 netbluemind4-4.9.2928/netbluemind/core/api/date/
--rw-r--r--   0 root         (0) root         (0)     2417 2023-07-19 06:58:47.000000 netbluemind4-4.9.2928/netbluemind/core/api/date/BmDateTime.py
--rw-r--r--   0 root         (0) root         (0)     1122 2023-07-19 06:58:47.000000 netbluemind4-4.9.2928/netbluemind/core/api/date/BmDateTimePrecision.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:02.000000 netbluemind4-4.9.2928/netbluemind/core/api/date/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.291157 netbluemind4-4.9.2928/netbluemind/core/api/fault/
--rw-r--r--   0 root         (0) root         (0)     5090 2023-07-19 06:58:48.000000 netbluemind4-4.9.2928/netbluemind/core/api/fault/ErrorCode.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:02.000000 netbluemind4-4.9.2928/netbluemind/core/api/fault/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.291157 netbluemind4-4.9.2928/netbluemind/core/container/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:06.000000 netbluemind4-4.9.2928/netbluemind/core/container/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.295157 netbluemind4-4.9.2928/netbluemind/core/container/api/
--rw-r--r--   0 root         (0) root         (0)     1490 2023-07-19 06:58:45.000000 netbluemind4-4.9.2928/netbluemind/core/container/api/Ack.py
--rw-r--r--   0 root         (0) root         (0)     2318 2023-07-19 06:58:44.000000 netbluemind4-4.9.2928/netbluemind/core/container/api/ContainerHierarchyNode.py
--rw-r--r--   0 root         (0) root         (0)     2906 2023-07-19 06:58:46.000000 netbluemind4-4.9.2928/netbluemind/core/container/api/ContainerQuery.py
--rw-r--r--   0 root         (0) root         (0)     1862 2023-07-19 06:58:44.000000 netbluemind4-4.9.2928/netbluemind/core/container/api/ContainerSubscription.py
--rw-r--r--   0 root         (0) root         (0)     2460 2023-07-19 06:58:44.000000 netbluemind4-4.9.2928/netbluemind/core/container/api/ContainerSubscriptionDescriptor.py
--rw-r--r--   0 root         (0) root         (0)     2762 2023-07-19 06:58:45.000000 netbluemind4-4.9.2928/netbluemind/core/container/api/ContainerSubscriptionModel.py
--rw-r--r--   0 root         (0) root         (0)     1478 2023-07-19 06:58:45.000000 netbluemind4-4.9.2928/netbluemind/core/container/api/Count.py
--rw-r--r--   0 root         (0) root         (0)     6266 2023-07-19 06:58:45.000000 netbluemind4-4.9.2928/netbluemind/core/container/api/IChangelogSupport.py
--rw-r--r--   0 root         (0) root         (0)    10791 2023-07-19 06:58:46.000000 netbluemind4-4.9.2928/netbluemind/core/container/api/IContainerManagement.py
--rw-r--r--   0 root         (0) root         (0)     2974 2023-07-19 06:58:46.000000 netbluemind4-4.9.2928/netbluemind/core/container/api/IContainerSync.py
--rw-r--r--   0 root         (0) root         (0)    10675 2023-07-19 06:58:44.000000 netbluemind4-4.9.2928/netbluemind/core/container/api/IContainers.py
--rw-r--r--   0 root         (0) root         (0)    10290 2023-07-19 06:58:46.000000 netbluemind4-4.9.2928/netbluemind/core/container/api/IContainersFlatHierarchy.py
--rw-r--r--   0 root         (0) root         (0)     1788 2023-07-19 06:58:47.000000 netbluemind4-4.9.2928/netbluemind/core/container/api/ICountingSupport.py
--rw-r--r--   0 root         (0) root         (0)     1529 2023-07-19 06:58:46.000000 netbluemind4-4.9.2928/netbluemind/core/container/api/IFlatHierarchyUids.py
--rw-r--r--   0 root         (0) root         (0)     1799 2023-07-19 06:58:45.000000 netbluemind4-4.9.2928/netbluemind/core/container/api/IOfflineMgmt.py
--rw-r--r--   0 root         (0) root         (0)     1543 2023-07-19 06:58:44.000000 netbluemind4-4.9.2928/netbluemind/core/container/api/IOwnerSubscriptionUids.py
--rw-r--r--   0 root         (0) root         (0)    12217 2023-07-19 06:58:47.000000 netbluemind4-4.9.2928/netbluemind/core/container/api/IOwnerSubscriptions.py
--rw-r--r--   0 root         (0) root         (0)     1667 2023-07-19 06:58:44.000000 netbluemind4-4.9.2928/netbluemind/core/container/api/ISortingSupport.py
--rw-r--r--   0 root         (0) root         (0)     1763 2023-07-19 06:58:44.000000 netbluemind4-4.9.2928/netbluemind/core/container/api/IdRange.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:06.000000 netbluemind4-4.9.2928/netbluemind/core/container/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.303158 netbluemind4-4.9.2928/netbluemind/core/container/model/
--rw-r--r--   0 root         (0) root         (0)     4440 2023-07-19 06:58:43.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/BaseContainerDescriptor.py
--rw-r--r--   0 root         (0) root         (0)     3777 2023-07-19 06:58:43.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/ChangeLogEntry.py
--rw-r--r--   0 root         (0) root         (0)     1147 2023-07-19 06:58:43.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/ChangeLogEntryType.py
--rw-r--r--   0 root         (0) root         (0)     1981 2023-07-19 06:58:43.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/ContainerChangelog.py
--rw-r--r--   0 root         (0) root         (0)     2477 2023-07-19 06:58:43.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/ContainerChangeset.py
--rw-r--r--   0 root         (0) root         (0)     3053 2023-07-19 06:58:43.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/ContainerDescriptor.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-07-19 06:58:43.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/ContainerModifiableDescriptor.py
--rw-r--r--   0 root         (0) root         (0)     2861 2023-07-19 06:58:43.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/ContainerSyncResult.py
--rw-r--r--   0 root         (0) root         (0)     3156 2023-07-19 06:58:43.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/ContainerSyncStatus.py
--rw-r--r--   0 root         (0) root         (0)     1140 2023-07-19 06:58:43.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/ContainerSyncStatusStatus.py
--rw-r--r--   0 root         (0) root         (0)     3489 2023-07-19 06:58:43.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/ContainerUpdatesResult.py
--rw-r--r--   0 root         (0) root         (0)     2320 2023-07-19 06:58:43.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/ContainerUpdatesResultInError.py
--rw-r--r--   0 root         (0) root         (0)     2677 2023-07-19 06:58:43.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/IdQuery.py
--rw-r--r--   0 root         (0) root         (0)     2004 2023-07-19 06:58:43.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/ItemChangeLogEntry.py
--rw-r--r--   0 root         (0) root         (0)     2006 2023-07-19 06:58:43.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/ItemChangelog.py
--rw-r--r--   0 root         (0) root         (0)     3737 2023-07-19 06:58:43.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/ItemContainerValue.py
--rw-r--r--   0 root         (0) root         (0)     4056 2023-07-19 06:58:43.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/ItemDescriptor.py
--rw-r--r--   0 root         (0) root         (0)     1115 2023-07-19 06:58:43.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/ItemFlag.py
--rw-r--r--   0 root         (0) root         (0)     2853 2023-07-19 06:58:43.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/ItemFlagFilter.py
--rw-r--r--   0 root         (0) root         (0)     1816 2023-07-19 06:58:43.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/ItemIdentifier.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-07-19 06:58:43.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/ItemUri.py
--rw-r--r--   0 root         (0) root         (0)     4295 2023-07-19 06:58:43.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/ItemValue.py
--rw-r--r--   0 root         (0) root         (0)     1696 2023-07-19 06:58:43.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/ItemVersion.py
--rw-r--r--   0 root         (0) root         (0)     2010 2023-07-19 06:58:43.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/SortDescriptor.py
--rw-r--r--   0 root         (0) root         (0)     1124 2023-07-19 06:58:43.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/SortDescriptorDirection.py
--rw-r--r--   0 root         (0) root         (0)     2196 2023-07-19 06:58:43.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/SortDescriptorField.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:06.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.303158 netbluemind4-4.9.2928/netbluemind/core/container/model/acl/
--rw-r--r--   0 root         (0) root         (0)     2037 2023-07-19 06:58:44.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/acl/AccessControlEntry.py
--rw-r--r--   0 root         (0) root         (0)     1199 2023-07-19 06:58:44.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/acl/Verb.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:06.000000 netbluemind4-4.9.2928/netbluemind/core/container/model/acl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.303158 netbluemind4-4.9.2928/netbluemind/core/task/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:06.000000 netbluemind4-4.9.2928/netbluemind/core/task/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.303158 netbluemind4-4.9.2928/netbluemind/core/task/api/
--rw-r--r--   0 root         (0) root         (0)     2471 2023-07-19 06:58:47.000000 netbluemind4-4.9.2928/netbluemind/core/task/api/ITask.py
--rw-r--r--   0 root         (0) root         (0)     1461 2023-07-19 06:58:47.000000 netbluemind4-4.9.2928/netbluemind/core/task/api/TaskRef.py
--rw-r--r--   0 root         (0) root         (0)     2808 2023-07-19 06:58:47.000000 netbluemind4-4.9.2928/netbluemind/core/task/api/TaskStatus.py
--rw-r--r--   0 root         (0) root         (0)     1174 2023-07-19 06:58:47.000000 netbluemind4-4.9.2928/netbluemind/core/task/api/TaskStatusState.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:06.000000 netbluemind4-4.9.2928/netbluemind/core/task/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.303158 netbluemind4-4.9.2928/netbluemind/cti/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:06.000000 netbluemind4-4.9.2928/netbluemind/cti/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.307158 netbluemind4-4.9.2928/netbluemind/cti/api/
--rw-r--r--   0 root         (0) root         (0)     4038 2023-07-19 06:58:48.000000 netbluemind4-4.9.2928/netbluemind/cti/api/IComputerTelephonyIntegration.py
--rw-r--r--   0 root         (0) root         (0)     2610 2023-07-19 06:58:48.000000 netbluemind4-4.9.2928/netbluemind/cti/api/Status.py
--rw-r--r--   0 root         (0) root         (0)     1219 2023-07-19 06:58:48.000000 netbluemind4-4.9.2928/netbluemind/cti/api/StatusPhoneState.py
--rw-r--r--   0 root         (0) root         (0)     1155 2023-07-19 06:58:48.000000 netbluemind4-4.9.2928/netbluemind/cti/api/StatusType.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:06.000000 netbluemind4-4.9.2928/netbluemind/cti/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.307158 netbluemind4-4.9.2928/netbluemind/dataprotect/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:06.000000 netbluemind4-4.9.2928/netbluemind/dataprotect/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.311158 netbluemind4-4.9.2928/netbluemind/dataprotect/api/
--rw-r--r--   0 root         (0) root         (0)     3500 2023-07-19 06:58:48.000000 netbluemind4-4.9.2928/netbluemind/dataprotect/api/DataProtectGeneration.py
--rw-r--r--   0 root         (0) root         (0)     4139 2023-07-19 06:58:48.000000 netbluemind4-4.9.2928/netbluemind/dataprotect/api/GenerationContent.py
--rw-r--r--   0 root         (0) root         (0)     1137 2023-07-19 06:58:49.000000 netbluemind4-4.9.2928/netbluemind/dataprotect/api/GenerationStatus.py
--rw-r--r--   0 root         (0) root         (0)     8292 2023-07-19 06:58:49.000000 netbluemind4-4.9.2928/netbluemind/dataprotect/api/IDataProtect.py
--rw-r--r--   0 root         (0) root         (0)     4132 2023-07-19 06:58:48.000000 netbluemind4-4.9.2928/netbluemind/dataprotect/api/PartGeneration.py
--rw-r--r--   0 root         (0) root         (0)     2878 2023-07-19 06:58:48.000000 netbluemind4-4.9.2928/netbluemind/dataprotect/api/Restorable.py
--rw-r--r--   0 root         (0) root         (0)     1229 2023-07-19 06:58:49.000000 netbluemind4-4.9.2928/netbluemind/dataprotect/api/RestorableKind.py
--rw-r--r--   0 root         (0) root         (0)     2507 2023-07-19 06:58:48.000000 netbluemind4-4.9.2928/netbluemind/dataprotect/api/RestoreDefinition.py
--rw-r--r--   0 root         (0) root         (0)     2389 2023-07-19 06:58:48.000000 netbluemind4-4.9.2928/netbluemind/dataprotect/api/RestoreOperation.py
--rw-r--r--   0 root         (0) root         (0)     1947 2023-07-19 06:58:49.000000 netbluemind4-4.9.2928/netbluemind/dataprotect/api/RetentionPolicy.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:06.000000 netbluemind4-4.9.2928/netbluemind/dataprotect/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.311158 netbluemind4-4.9.2928/netbluemind/device/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:06.000000 netbluemind4-4.9.2928/netbluemind/device/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.311158 netbluemind4-4.9.2928/netbluemind/device/api/
--rw-r--r--   0 root         (0) root         (0)     3871 2023-07-19 06:58:42.000000 netbluemind4-4.9.2928/netbluemind/device/api/Device.py
--rw-r--r--   0 root         (0) root         (0)     8350 2023-07-19 06:58:42.000000 netbluemind4-4.9.2928/netbluemind/device/api/IDevice.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-07-19 06:58:42.000000 netbluemind4-4.9.2928/netbluemind/device/api/IDeviceUids.py
--rw-r--r--   0 root         (0) root         (0)     1498 2023-07-19 06:58:42.000000 netbluemind4-4.9.2928/netbluemind/device/api/IDevices.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:06.000000 netbluemind4-4.9.2928/netbluemind/device/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.311158 netbluemind4-4.9.2928/netbluemind/directory/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:06.000000 netbluemind4-4.9.2928/netbluemind/directory/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.315158 netbluemind4-4.9.2928/netbluemind/directory/api/
--rw-r--r--   0 root         (0) root         (0)     3091 2023-07-19 06:59:13.000000 netbluemind4-4.9.2928/netbluemind/directory/api/BaseDirEntry.py
--rw-r--r--   0 root         (0) root         (0)     1168 2023-07-19 06:59:13.000000 netbluemind4-4.9.2928/netbluemind/directory/api/BaseDirEntryAccountType.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-07-19 06:59:13.000000 netbluemind4-4.9.2928/netbluemind/directory/api/BaseDirEntryKind.py
--rw-r--r--   0 root         (0) root         (0)     3052 2023-07-19 06:59:13.000000 netbluemind4-4.9.2928/netbluemind/directory/api/DirBaseValue.py
--rw-r--r--   0 root         (0) root         (0)     4364 2023-07-19 06:59:13.000000 netbluemind4-4.9.2928/netbluemind/directory/api/DirEntry.py
--rw-r--r--   0 root         (0) root         (0)     7466 2023-07-19 06:59:14.000000 netbluemind4-4.9.2928/netbluemind/directory/api/DirEntryQuery.py
--rw-r--r--   0 root         (0) root         (0)     1103 2023-07-19 06:59:13.000000 netbluemind4-4.9.2928/netbluemind/directory/api/DirEntryQueryDir.py
--rw-r--r--   0 root         (0) root         (0)     2469 2023-07-19 06:59:13.000000 netbluemind4-4.9.2928/netbluemind/directory/api/DirEntryQueryOrder.py
--rw-r--r--   0 root         (0) root         (0)     1131 2023-07-19 06:59:13.000000 netbluemind4-4.9.2928/netbluemind/directory/api/DirEntryQueryOrderBy.py
--rw-r--r--   0 root         (0) root         (0)     1157 2023-07-19 06:59:13.000000 netbluemind4-4.9.2928/netbluemind/directory/api/DirEntryQueryStateFilter.py
--rw-r--r--   0 root         (0) root         (0)     2719 2023-07-19 06:59:14.000000 netbluemind4-4.9.2928/netbluemind/directory/api/IDirEntryMaintenance.py
--rw-r--r--   0 root         (0) root         (0)     1507 2023-07-19 06:59:14.000000 netbluemind4-4.9.2928/netbluemind/directory/api/IDirEntryPath.py
--rw-r--r--   0 root         (0) root         (0)    14188 2023-07-19 06:59:13.000000 netbluemind4-4.9.2928/netbluemind/directory/api/IDirectory.py
--rw-r--r--   0 root         (0) root         (0)     9345 2023-07-19 06:59:14.000000 netbluemind4-4.9.2928/netbluemind/directory/api/IOrgUnits.py
--rw-r--r--   0 root         (0) root         (0)     1839 2023-07-19 06:59:13.000000 netbluemind4-4.9.2928/netbluemind/directory/api/MaintenanceOperation.py
--rw-r--r--   0 root         (0) root         (0)     1728 2023-07-19 06:59:13.000000 netbluemind4-4.9.2928/netbluemind/directory/api/OrgUnit.py
--rw-r--r--   0 root         (0) root         (0)     2228 2023-07-19 06:59:13.000000 netbluemind4-4.9.2928/netbluemind/directory/api/OrgUnitPath.py
--rw-r--r--   0 root         (0) root         (0)     2632 2023-07-19 06:59:13.000000 netbluemind4-4.9.2928/netbluemind/directory/api/OrgUnitQuery.py
--rw-r--r--   0 root         (0) root         (0)     2345 2023-07-19 06:59:14.000000 netbluemind4-4.9.2928/netbluemind/directory/api/RepairConfig.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:06.000000 netbluemind4-4.9.2928/netbluemind/directory/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.315158 netbluemind4-4.9.2928/netbluemind/document/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:06.000000 netbluemind4-4.9.2928/netbluemind/document/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.315158 netbluemind4-4.9.2928/netbluemind/document/api/
--rw-r--r--   0 root         (0) root         (0)     2146 2023-07-19 06:58:41.000000 netbluemind4-4.9.2928/netbluemind/document/api/Document.py
--rw-r--r--   0 root         (0) root         (0)     2412 2023-07-19 06:58:42.000000 netbluemind4-4.9.2928/netbluemind/document/api/DocumentMetadata.py
--rw-r--r--   0 root         (0) root         (0)     5027 2023-07-19 06:58:42.000000 netbluemind4-4.9.2928/netbluemind/document/api/IDocument.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:06.000000 netbluemind4-4.9.2928/netbluemind/document/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.315158 netbluemind4-4.9.2928/netbluemind/documentfolder/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:06.000000 netbluemind4-4.9.2928/netbluemind/documentfolder/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.315158 netbluemind4-4.9.2928/netbluemind/documentfolder/api/
--rw-r--r--   0 root         (0) root         (0)     1695 2023-07-19 06:58:41.000000 netbluemind4-4.9.2928/netbluemind/documentfolder/api/DocumentFolder.py
--rw-r--r--   0 root         (0) root         (0)     4166 2023-07-19 06:58:41.000000 netbluemind4-4.9.2928/netbluemind/documentfolder/api/IDocumentFolder.py
--rw-r--r--   0 root         (0) root         (0)     1482 2023-07-19 06:58:41.000000 netbluemind4-4.9.2928/netbluemind/documentfolder/api/IDocumentFolderUids.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:06.000000 netbluemind4-4.9.2928/netbluemind/documentfolder/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.319158 netbluemind4-4.9.2928/netbluemind/domain/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:06.000000 netbluemind4-4.9.2928/netbluemind/domain/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.319158 netbluemind4-4.9.2928/netbluemind/domain/api/
--rw-r--r--   0 root         (0) root         (0)     3063 2023-07-19 06:59:02.000000 netbluemind4-4.9.2928/netbluemind/domain/api/Domain.py
--rw-r--r--   0 root         (0) root         (0)     2076 2023-07-19 06:59:02.000000 netbluemind4-4.9.2928/netbluemind/domain/api/IDomainSettings.py
--rw-r--r--   0 root         (0) root         (0)     8252 2023-07-19 06:59:02.000000 netbluemind4-4.9.2928/netbluemind/domain/api/IDomains.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:06.000000 netbluemind4-4.9.2928/netbluemind/domain/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.319158 netbluemind4-4.9.2928/netbluemind/eas/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:06.000000 netbluemind4-4.9.2928/netbluemind/eas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.319158 netbluemind4-4.9.2928/netbluemind/eas/api/
--rw-r--r--   0 root         (0) root         (0)     1728 2023-07-19 06:58:56.000000 netbluemind4-4.9.2928/netbluemind/eas/api/Account.py
--rw-r--r--   0 root         (0) root         (0)     2097 2023-07-19 06:58:56.000000 netbluemind4-4.9.2928/netbluemind/eas/api/FolderSyncVersions.py
--rw-r--r--   0 root         (0) root         (0)     1739 2023-07-19 06:58:56.000000 netbluemind4-4.9.2928/netbluemind/eas/api/Heartbeat.py
--rw-r--r--   0 root         (0) root         (0)     7128 2023-07-19 06:58:56.000000 netbluemind4-4.9.2928/netbluemind/eas/api/IEas.py
--rw-r--r--   0 root         (0) root         (0)     1920 2023-07-19 06:58:56.000000 netbluemind4-4.9.2928/netbluemind/eas/api/SentItem.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:06.000000 netbluemind4-4.9.2928/netbluemind/eas/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.319158 netbluemind4-4.9.2928/netbluemind/externaluser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:10.000000 netbluemind4-4.9.2928/netbluemind/externaluser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.319158 netbluemind4-4.9.2928/netbluemind/externaluser/api/
--rw-r--r--   0 root         (0) root         (0)     2153 2023-07-19 06:58:59.000000 netbluemind4-4.9.2928/netbluemind/externaluser/api/ExternalUser.py
--rw-r--r--   0 root         (0) root         (0)     6976 2023-07-19 06:59:00.000000 netbluemind4-4.9.2928/netbluemind/externaluser/api/IExternalUser.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:10.000000 netbluemind4-4.9.2928/netbluemind/externaluser/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.319158 netbluemind4-4.9.2928/netbluemind/filehosting/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/filehosting/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.323158 netbluemind4-4.9.2928/netbluemind/filehosting/api/
--rw-r--r--   0 root         (0) root         (0)     1835 2023-07-19 06:58:40.000000 netbluemind4-4.9.2928/netbluemind/filehosting/api/Configuration.py
--rw-r--r--   0 root         (0) root         (0)     2348 2023-07-19 06:58:40.000000 netbluemind4-4.9.2928/netbluemind/filehosting/api/FileHostingInfo.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-07-19 06:58:41.000000 netbluemind4-4.9.2928/netbluemind/filehosting/api/FileHostingInfoType.py
--rw-r--r--   0 root         (0) root         (0)     3011 2023-07-19 06:58:41.000000 netbluemind4-4.9.2928/netbluemind/filehosting/api/FileHostingItem.py
--rw-r--r--   0 root         (0) root         (0)     1802 2023-07-19 06:58:40.000000 netbluemind4-4.9.2928/netbluemind/filehosting/api/FileHostingPublicLink.py
--rw-r--r--   0 root         (0) root         (0)     1091 2023-07-19 06:58:41.000000 netbluemind4-4.9.2928/netbluemind/filehosting/api/FileType.py
--rw-r--r--   0 root         (0) root         (0)     8093 2023-07-19 06:58:41.000000 netbluemind4-4.9.2928/netbluemind/filehosting/api/IFileHosting.py
--rw-r--r--   0 root         (0) root         (0)     1515 2023-07-19 06:58:41.000000 netbluemind4-4.9.2928/netbluemind/filehosting/api/IInternalBMFileSystem.py
--rw-r--r--   0 root         (0) root         (0)     1686 2023-07-19 06:58:40.000000 netbluemind4-4.9.2928/netbluemind/filehosting/api/Metadata.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/filehosting/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.323158 netbluemind4-4.9.2928/netbluemind/group/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/group/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.323158 netbluemind4-4.9.2928/netbluemind/group/api/
--rw-r--r--   0 root         (0) root         (0)     3205 2023-07-19 06:58:51.000000 netbluemind4-4.9.2928/netbluemind/group/api/Group.py
--rw-r--r--   0 root         (0) root         (0)     1826 2023-07-19 06:58:51.000000 netbluemind4-4.9.2928/netbluemind/group/api/GroupSearchQuery.py
--rw-r--r--   0 root         (0) root         (0)    16842 2023-07-19 06:58:51.000000 netbluemind4-4.9.2928/netbluemind/group/api/IGroup.py
--rw-r--r--   0 root         (0) root         (0)     2253 2023-07-19 06:58:50.000000 netbluemind4-4.9.2928/netbluemind/group/api/IGroupMember.py
--rw-r--r--   0 root         (0) root         (0)     1965 2023-07-19 06:58:51.000000 netbluemind4-4.9.2928/netbluemind/group/api/Member.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-07-19 06:58:51.000000 netbluemind4-4.9.2928/netbluemind/group/api/MemberType.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/group/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.323158 netbluemind4-4.9.2928/netbluemind/hsm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/hsm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.327158 netbluemind4-4.9.2928/netbluemind/hsm/api/
--rw-r--r--   0 root         (0) root         (0)     1968 2023-07-19 06:58:51.000000 netbluemind4-4.9.2928/netbluemind/hsm/api/Demote.py
--rw-r--r--   0 root         (0) root         (0)     3771 2023-07-19 06:58:52.000000 netbluemind4-4.9.2928/netbluemind/hsm/api/IHSM.py
--rw-r--r--   0 root         (0) root         (0)     2714 2023-07-19 06:58:52.000000 netbluemind4-4.9.2928/netbluemind/hsm/api/Promote.py
--rw-r--r--   0 root         (0) root         (0)     1731 2023-07-19 06:58:52.000000 netbluemind4-4.9.2928/netbluemind/hsm/api/TierChangeResult.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/hsm/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.327158 netbluemind4-4.9.2928/netbluemind/icalendar/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/icalendar/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.331158 netbluemind4-4.9.2928/netbluemind/icalendar/api/
--rw-r--r--   0 root         (0) root         (0)    11482 2023-07-19 06:59:07.000000 netbluemind4-4.9.2928/netbluemind/icalendar/api/ICalendarElement.py
--rw-r--r--   0 root         (0) root         (0)     6703 2023-07-19 06:59:07.000000 netbluemind4-4.9.2928/netbluemind/icalendar/api/ICalendarElementAttendee.py
--rw-r--r--   0 root         (0) root         (0)     1205 2023-07-19 06:59:07.000000 netbluemind4-4.9.2928/netbluemind/icalendar/api/ICalendarElementCUType.py
--rw-r--r--   0 root         (0) root         (0)     1191 2023-07-19 06:59:07.000000 netbluemind4-4.9.2928/netbluemind/icalendar/api/ICalendarElementClassification.py
--rw-r--r--   0 root         (0) root         (0)     2199 2023-07-19 06:59:07.000000 netbluemind4-4.9.2928/netbluemind/icalendar/api/ICalendarElementOrganizer.py
--rw-r--r--   0 root         (0) root         (0)     1294 2023-07-19 06:59:07.000000 netbluemind4-4.9.2928/netbluemind/icalendar/api/ICalendarElementParticipationStatus.py
--rw-r--r--   0 root         (0) root         (0)     6113 2023-07-19 06:59:07.000000 netbluemind4-4.9.2928/netbluemind/icalendar/api/ICalendarElementRRule.py
--rw-r--r--   0 root         (0) root         (0)     1273 2023-07-19 06:59:07.000000 netbluemind4-4.9.2928/netbluemind/icalendar/api/ICalendarElementRRuleFrequency.py
--rw-r--r--   0 root         (0) root         (0)     1749 2023-07-19 06:59:07.000000 netbluemind4-4.9.2928/netbluemind/icalendar/api/ICalendarElementRRuleWeekDay.py
--rw-r--r--   0 root         (0) root         (0)     1235 2023-07-19 06:59:07.000000 netbluemind4-4.9.2928/netbluemind/icalendar/api/ICalendarElementRole.py
--rw-r--r--   0 root         (0) root         (0)     1259 2023-07-19 06:59:07.000000 netbluemind4-4.9.2928/netbluemind/icalendar/api/ICalendarElementStatus.py
--rw-r--r--   0 root         (0) root         (0)     3218 2023-07-19 06:59:07.000000 netbluemind4-4.9.2928/netbluemind/icalendar/api/ICalendarElementVAlarm.py
--rw-r--r--   0 root         (0) root         (0)     1169 2023-07-19 06:59:07.000000 netbluemind4-4.9.2928/netbluemind/icalendar/api/ICalendarElementVAlarmAction.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/icalendar/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.331158 netbluemind4-4.9.2928/netbluemind/im/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/im/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.331158 netbluemind4-4.9.2928/netbluemind/im/api/
--rw-r--r--   0 root         (0) root         (0)     3937 2023-07-19 06:58:26.000000 netbluemind4-4.9.2928/netbluemind/im/api/IInstantMessaging.py
--rw-r--r--   0 root         (0) root         (0)     2127 2023-07-19 06:58:26.000000 netbluemind4-4.9.2928/netbluemind/im/api/IMMessage.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/im/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.331158 netbluemind4-4.9.2928/netbluemind/mailbox/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/mailbox/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.335158 netbluemind4-4.9.2928/netbluemind/mailbox/api/
--rw-r--r--   0 root         (0) root         (0)     1444 2023-07-19 06:58:56.000000 netbluemind4-4.9.2928/netbluemind/mailbox/api/IMailboxAclUids.py
--rw-r--r--   0 root         (0) root         (0)     5008 2023-07-19 06:58:57.000000 netbluemind4-4.9.2928/netbluemind/mailbox/api/IMailboxMgmt.py
--rw-r--r--   0 root         (0) root         (0)    17092 2023-07-19 06:58:58.000000 netbluemind4-4.9.2928/netbluemind/mailbox/api/IMailboxes.py
--rw-r--r--   0 root         (0) root         (0)     3211 2023-07-19 06:58:58.000000 netbluemind4-4.9.2928/netbluemind/mailbox/api/MailFilter.py
--rw-r--r--   0 root         (0) root         (0)     2069 2023-07-19 06:58:56.000000 netbluemind4-4.9.2928/netbluemind/mailbox/api/MailFilterForwarding.py
--rw-r--r--   0 root         (0) root         (0)     3916 2023-07-19 06:58:56.000000 netbluemind4-4.9.2928/netbluemind/mailbox/api/MailFilterRule.py
--rw-r--r--   0 root         (0) root         (0)     2616 2023-07-19 06:58:56.000000 netbluemind4-4.9.2928/netbluemind/mailbox/api/MailFilterVacation.py
--rw-r--r--   0 root         (0) root         (0)     4279 2023-07-19 06:58:56.000000 netbluemind4-4.9.2928/netbluemind/mailbox/api/Mailbox.py
--rw-r--r--   0 root         (0) root         (0)     1788 2023-07-19 06:58:58.000000 netbluemind4-4.9.2928/netbluemind/mailbox/api/MailboxConfig.py
--rw-r--r--   0 root         (0) root         (0)     1695 2023-07-19 06:58:57.000000 netbluemind4-4.9.2928/netbluemind/mailbox/api/MailboxQuota.py
--rw-r--r--   0 root         (0) root         (0)     1133 2023-07-19 06:58:56.000000 netbluemind4-4.9.2928/netbluemind/mailbox/api/MailboxRouting.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-07-19 06:58:57.000000 netbluemind4-4.9.2928/netbluemind/mailbox/api/MailboxType.py
--rw-r--r--   0 root         (0) root         (0)     2940 2023-07-19 06:58:56.000000 netbluemind4-4.9.2928/netbluemind/mailbox/api/ShardStats.py
--rw-r--r--   0 root         (0) root         (0)     1814 2023-07-19 06:58:56.000000 netbluemind4-4.9.2928/netbluemind/mailbox/api/ShardStatsMailboxStats.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-07-19 06:58:58.000000 netbluemind4-4.9.2928/netbluemind/mailbox/api/ShardStatsState.py
--rw-r--r--   0 root         (0) root         (0)     3337 2023-07-19 06:58:58.000000 netbluemind4-4.9.2928/netbluemind/mailbox/api/SimpleShardStats.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/mailbox/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.335158 netbluemind4-4.9.2928/netbluemind/mailbox/identity/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/mailbox/identity/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.335158 netbluemind4-4.9.2928/netbluemind/mailbox/identity/api/
--rw-r--r--   0 root         (0) root         (0)     5175 2023-07-19 06:58:58.000000 netbluemind4-4.9.2928/netbluemind/mailbox/identity/api/IMailboxIdentity.py
--rw-r--r--   0 root         (0) root         (0)     3330 2023-07-19 06:58:58.000000 netbluemind4-4.9.2928/netbluemind/mailbox/identity/api/Identity.py
--rw-r--r--   0 root         (0) root         (0)     3125 2023-07-19 06:58:58.000000 netbluemind4-4.9.2928/netbluemind/mailbox/identity/api/IdentityDescription.py
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-19 06:58:58.000000 netbluemind4-4.9.2928/netbluemind/mailbox/identity/api/SignatureFormat.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/mailbox/identity/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.335158 netbluemind4-4.9.2928/netbluemind/mailflow/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/mailflow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.335158 netbluemind4-4.9.2928/netbluemind/mailflow/common/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/mailflow/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.335158 netbluemind4-4.9.2928/netbluemind/mailflow/common/api/
--rw-r--r--   0 root         (0) root         (0)     2218 2023-07-19 06:58:48.000000 netbluemind4-4.9.2928/netbluemind/mailflow/common/api/AssignmentActionMapping.py
--rw-r--r--   0 root         (0) root         (0)     2849 2023-07-19 06:58:48.000000 netbluemind4-4.9.2928/netbluemind/mailflow/common/api/Message.py
--rw-r--r--   0 root         (0) root         (0)     3164 2023-07-19 06:58:48.000000 netbluemind4-4.9.2928/netbluemind/mailflow/common/api/Recipient.py
--rw-r--r--   0 root         (0) root         (0)     1127 2023-07-19 06:58:48.000000 netbluemind4-4.9.2928/netbluemind/mailflow/common/api/RecipientAddressType.py
--rw-r--r--   0 root         (0) root         (0)     1131 2023-07-19 06:58:48.000000 netbluemind4-4.9.2928/netbluemind/mailflow/common/api/RecipientRecipientType.py
--rw-r--r--   0 root         (0) root         (0)     1714 2023-07-19 06:58:48.000000 netbluemind4-4.9.2928/netbluemind/mailflow/common/api/SendingAs.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/mailflow/common/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.335158 netbluemind4-4.9.2928/netbluemind/mailmessage/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/mailmessage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.339158 netbluemind4-4.9.2928/netbluemind/mailmessage/api/
--rw-r--r--   0 root         (0) root         (0)     1928 2023-07-19 06:59:07.000000 netbluemind4-4.9.2928/netbluemind/mailmessage/api/IMailTip.py
--rw-r--r--   0 root         (0) root         (0)     1755 2023-07-19 06:59:07.000000 netbluemind4-4.9.2928/netbluemind/mailmessage/api/MailTip.py
--rw-r--r--   0 root         (0) root         (0)     2531 2023-07-19 06:59:07.000000 netbluemind4-4.9.2928/netbluemind/mailmessage/api/MailTipContext.py
--rw-r--r--   0 root         (0) root         (0)     2316 2023-07-19 06:59:07.000000 netbluemind4-4.9.2928/netbluemind/mailmessage/api/MailTipFilter.py
--rw-r--r--   0 root         (0) root         (0)     1138 2023-07-19 06:59:07.000000 netbluemind4-4.9.2928/netbluemind/mailmessage/api/MailTipFilterFilterType.py
--rw-r--r--   0 root         (0) root         (0)     2519 2023-07-19 06:59:07.000000 netbluemind4-4.9.2928/netbluemind/mailmessage/api/MailTips.py
--rw-r--r--   0 root         (0) root         (0)     3062 2023-07-19 06:59:07.000000 netbluemind4-4.9.2928/netbluemind/mailmessage/api/MessageContext.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/mailmessage/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.339158 netbluemind4-4.9.2928/netbluemind/mailshare/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/mailshare/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.339158 netbluemind4-4.9.2928/netbluemind/mailshare/api/
--rw-r--r--   0 root         (0) root         (0)     6859 2023-07-19 06:58:50.000000 netbluemind4-4.9.2928/netbluemind/mailshare/api/IMailshare.py
--rw-r--r--   0 root         (0) root         (0)     3056 2023-07-19 06:58:50.000000 netbluemind4-4.9.2928/netbluemind/mailshare/api/Mailshare.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/mailshare/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.339158 netbluemind4-4.9.2928/netbluemind/notes/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:10.000000 netbluemind4-4.9.2928/netbluemind/notes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.343159 netbluemind4-4.9.2928/netbluemind/notes/api/
--rw-r--r--   0 root         (0) root         (0)    19475 2023-07-19 06:58:40.000000 netbluemind4-4.9.2928/netbluemind/notes/api/INote.py
--rw-r--r--   0 root         (0) root         (0)     2192 2023-07-19 06:58:39.000000 netbluemind4-4.9.2928/netbluemind/notes/api/INoteIndexMgmt.py
--rw-r--r--   0 root         (0) root         (0)     1942 2023-07-19 06:58:40.000000 netbluemind4-4.9.2928/netbluemind/notes/api/INoteUids.py
--rw-r--r--   0 root         (0) root         (0)     3227 2023-07-19 06:58:39.000000 netbluemind4-4.9.2928/netbluemind/notes/api/INotes.py
--rw-r--r--   0 root         (0) root         (0)     3598 2023-07-19 06:58:40.000000 netbluemind4-4.9.2928/netbluemind/notes/api/VNote.py
--rw-r--r--   0 root         (0) root         (0)     3333 2023-07-19 06:58:40.000000 netbluemind4-4.9.2928/netbluemind/notes/api/VNoteChanges.py
--rw-r--r--   0 root         (0) root         (0)     2290 2023-07-19 06:58:39.000000 netbluemind4-4.9.2928/netbluemind/notes/api/VNoteChangesItemAdd.py
--rw-r--r--   0 root         (0) root         (0)     1842 2023-07-19 06:58:40.000000 netbluemind4-4.9.2928/netbluemind/notes/api/VNoteChangesItemDelete.py
--rw-r--r--   0 root         (0) root         (0)     2526 2023-07-19 06:58:40.000000 netbluemind4-4.9.2928/netbluemind/notes/api/VNoteChangesItemModify.py
--rw-r--r--   0 root         (0) root         (0)     1149 2023-07-19 06:58:40.000000 netbluemind4-4.9.2928/netbluemind/notes/api/VNoteColor.py
--rw-r--r--   0 root         (0) root         (0)     2169 2023-07-19 06:58:40.000000 netbluemind4-4.9.2928/netbluemind/notes/api/VNoteQuery.py
--rw-r--r--   0 root         (0) root         (0)     2374 2023-07-19 06:58:40.000000 netbluemind4-4.9.2928/netbluemind/notes/api/VNotesQuery.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:10.000000 netbluemind4-4.9.2928/netbluemind/notes/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.343159 netbluemind4-4.9.2928/netbluemind/python/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-23 11:00:08.000000 netbluemind4-4.9.2928/netbluemind/python/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4632 2023-07-19 06:58:50.000000 netbluemind4-4.9.2928/netbluemind/python/client.py
--rw-r--r--   0 root         (0) root         (0)     4129 2023-07-19 06:58:50.000000 netbluemind4-4.9.2928/netbluemind/python/serder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.343159 netbluemind4-4.9.2928/netbluemind/resource/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/resource/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.343159 netbluemind4-4.9.2928/netbluemind/resource/api/
--rw-r--r--   0 root         (0) root         (0)     1281 2023-07-19 06:58:52.000000 netbluemind4-4.9.2928/netbluemind/resource/api/EventInfo.py
--rw-r--r--   0 root         (0) root         (0)     7985 2023-07-19 06:58:52.000000 netbluemind4-4.9.2928/netbluemind/resource/api/IResources.py
--rw-r--r--   0 root         (0) root         (0)     3991 2023-07-19 06:58:52.000000 netbluemind4-4.9.2928/netbluemind/resource/api/ResourceDescriptor.py
--rw-r--r--   0 root         (0) root         (0)     1818 2023-07-19 06:58:52.000000 netbluemind4-4.9.2928/netbluemind/resource/api/ResourceDescriptorPropertyValue.py
--rw-r--r--   0 root         (0) root         (0)     1204 2023-07-19 06:58:52.000000 netbluemind4-4.9.2928/netbluemind/resource/api/ResourceReservationMode.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/resource/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.347159 netbluemind4-4.9.2928/netbluemind/resource/api/type/
--rw-r--r--   0 root         (0) root         (0)     1458 2023-07-19 06:58:52.000000 netbluemind4-4.9.2928/netbluemind/resource/api/type/IResourceTypeUids.py
--rw-r--r--   0 root         (0) root         (0)     5685 2023-07-19 06:58:53.000000 netbluemind4-4.9.2928/netbluemind/resource/api/type/IResourceTypes.py
--rw-r--r--   0 root         (0) root         (0)     1761 2023-07-19 06:58:53.000000 netbluemind4-4.9.2928/netbluemind/resource/api/type/ResourceType.py
--rw-r--r--   0 root         (0) root         (0)     2692 2023-07-19 06:58:52.000000 netbluemind4-4.9.2928/netbluemind/resource/api/type/ResourceTypeDescriptor.py
--rw-r--r--   0 root         (0) root         (0)     2526 2023-07-19 06:58:52.000000 netbluemind4-4.9.2928/netbluemind/resource/api/type/ResourceTypeDescriptorProperty.py
--rw-r--r--   0 root         (0) root         (0)     1191 2023-07-19 06:58:52.000000 netbluemind4-4.9.2928/netbluemind/resource/api/type/ResourceTypeDescriptorPropertyType.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/resource/api/type/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.347159 netbluemind4-4.9.2928/netbluemind/role/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/role/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.347159 netbluemind4-4.9.2928/netbluemind/role/api/
--rw-r--r--   0 root         (0) root         (0)     2151 2023-07-19 06:58:59.000000 netbluemind4-4.9.2928/netbluemind/role/api/IRoles.py
--rw-r--r--   0 root         (0) root         (0)     5403 2023-07-19 06:58:59.000000 netbluemind4-4.9.2928/netbluemind/role/api/RoleDescriptor.py
--rw-r--r--   0 root         (0) root         (0)     1926 2023-07-19 06:58:59.000000 netbluemind4-4.9.2928/netbluemind/role/api/RolesCategory.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/role/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.347159 netbluemind4-4.9.2928/netbluemind/scheduledjob/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/scheduledjob/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.351159 netbluemind4-4.9.2928/netbluemind/scheduledjob/api/
--rw-r--r--   0 root         (0) root         (0)     7252 2023-07-19 06:59:06.000000 netbluemind4-4.9.2928/netbluemind/scheduledjob/api/IJob.py
--rw-r--r--   0 root         (0) root         (0)     4227 2023-07-19 06:59:06.000000 netbluemind4-4.9.2928/netbluemind/scheduledjob/api/Job.py
--rw-r--r--   0 root         (0) root         (0)     2095 2023-07-19 06:59:06.000000 netbluemind4-4.9.2928/netbluemind/scheduledjob/api/JobDomainStatus.py
--rw-r--r--   0 root         (0) root         (0)     3227 2023-07-19 06:59:06.000000 netbluemind4-4.9.2928/netbluemind/scheduledjob/api/JobExecution.py
--rw-r--r--   0 root         (0) root         (0)     3201 2023-07-19 06:59:07.000000 netbluemind4-4.9.2928/netbluemind/scheduledjob/api/JobExecutionQuery.py
--rw-r--r--   0 root         (0) root         (0)     1252 2023-07-19 06:59:06.000000 netbluemind4-4.9.2928/netbluemind/scheduledjob/api/JobExitStatus.py
--rw-r--r--   0 root         (0) root         (0)     1096 2023-07-19 06:59:06.000000 netbluemind4-4.9.2928/netbluemind/scheduledjob/api/JobKind.py
--rw-r--r--   0 root         (0) root         (0)     2961 2023-07-19 06:59:07.000000 netbluemind4-4.9.2928/netbluemind/scheduledjob/api/JobPlanification.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-07-19 06:59:06.000000 netbluemind4-4.9.2928/netbluemind/scheduledjob/api/JobQuery.py
--rw-r--r--   0 root         (0) root         (0)     1530 2023-07-19 06:59:06.000000 netbluemind4-4.9.2928/netbluemind/scheduledjob/api/JobRec.py
--rw-r--r--   0 root         (0) root         (0)     2734 2023-07-19 06:59:07.000000 netbluemind4-4.9.2928/netbluemind/scheduledjob/api/LogEntry.py
--rw-r--r--   0 root         (0) root         (0)     1133 2023-07-19 06:59:06.000000 netbluemind4-4.9.2928/netbluemind/scheduledjob/api/LogLevel.py
--rw-r--r--   0 root         (0) root         (0)     1135 2023-07-19 06:59:06.000000 netbluemind4-4.9.2928/netbluemind/scheduledjob/api/PlanKind.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/scheduledjob/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.351159 netbluemind4-4.9.2928/netbluemind/server/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.351159 netbluemind4-4.9.2928/netbluemind/server/api/
--rw-r--r--   0 root         (0) root         (0)     1977 2023-07-19 06:58:58.000000 netbluemind4-4.9.2928/netbluemind/server/api/Assignment.py
--rw-r--r--   0 root         (0) root         (0)     2093 2023-07-19 06:58:59.000000 netbluemind4-4.9.2928/netbluemind/server/api/CommandStatus.py
--rw-r--r--   0 root         (0) root         (0)    12017 2023-07-19 06:58:59.000000 netbluemind4-4.9.2928/netbluemind/server/api/IServer.py
--rw-r--r--   0 root         (0) root         (0)     2108 2023-07-19 06:58:59.000000 netbluemind4-4.9.2928/netbluemind/server/api/Server.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:08.000000 netbluemind4-4.9.2928/netbluemind/server/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.351159 netbluemind4-4.9.2928/netbluemind/system/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:10.000000 netbluemind4-4.9.2928/netbluemind/system/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.359159 netbluemind4-4.9.2928/netbluemind/system/api/
--rw-r--r--   0 root         (0) root         (0)     3513 2023-07-19 06:59:11.000000 netbluemind4-4.9.2928/netbluemind/system/api/CertData.py
--rw-r--r--   0 root         (0) root         (0)     1192 2023-07-19 06:59:09.000000 netbluemind4-4.9.2928/netbluemind/system/api/CertDataCertificateDomainEngine.py
--rw-r--r--   0 root         (0) root         (0)     4088 2023-07-19 06:59:11.000000 netbluemind4-4.9.2928/netbluemind/system/api/CloneConfiguration.py
--rw-r--r--   0 root         (0) root         (0)     1147 2023-07-19 06:59:11.000000 netbluemind4-4.9.2928/netbluemind/system/api/CloneConfigurationMode.py
--rw-r--r--   0 root         (0) root         (0)     1147 2023-07-19 06:59:11.000000 netbluemind4-4.9.2928/netbluemind/system/api/ConnectionTestStatus.py
--rw-r--r--   0 root         (0) root         (0)     1764 2023-07-19 06:59:09.000000 netbluemind4-4.9.2928/netbluemind/system/api/CustomLogo.py
--rw-r--r--   0 root         (0) root         (0)     1951 2023-07-19 06:59:09.000000 netbluemind4-4.9.2928/netbluemind/system/api/DomainTemplate.py
--rw-r--r--   0 root         (0) root         (0)     2195 2023-07-19 06:59:11.000000 netbluemind4-4.9.2928/netbluemind/system/api/DomainTemplateDescription.py
--rw-r--r--   0 root         (0) root         (0)     2022 2023-07-19 06:59:11.000000 netbluemind4-4.9.2928/netbluemind/system/api/DomainTemplateDescriptionI18NDescription.py
--rw-r--r--   0 root         (0) root         (0)     2858 2023-07-19 06:59:11.000000 netbluemind4-4.9.2928/netbluemind/system/api/DomainTemplateKind.py
--rw-r--r--   0 root         (0) root         (0)     2999 2023-07-19 06:59:09.000000 netbluemind4-4.9.2928/netbluemind/system/api/DomainTemplateTag.py
--rw-r--r--   0 root         (0) root         (0)     2812 2023-07-19 06:59:12.000000 netbluemind4-4.9.2928/netbluemind/system/api/ExternalSystem.py
--rw-r--r--   0 root         (0) root         (0)     1209 2023-07-19 06:59:10.000000 netbluemind4-4.9.2928/netbluemind/system/api/ExternalSystemAuthKind.py
--rw-r--r--   0 root         (0) root         (0)     1764 2023-07-19 06:59:12.000000 netbluemind4-4.9.2928/netbluemind/system/api/ICacheMgmt.py
--rw-r--r--   0 root         (0) root         (0)     2464 2023-07-19 06:59:11.000000 netbluemind4-4.9.2928/netbluemind/system/api/ICustomTheme.py
--rw-r--r--   0 root         (0) root         (0)     1545 2023-07-19 06:59:11.000000 netbluemind4-4.9.2928/netbluemind/system/api/IDomainTemplate.py
--rw-r--r--   0 root         (0) root         (0)     4877 2023-07-19 06:59:09.000000 netbluemind4-4.9.2928/netbluemind/system/api/IExternalSystem.py
--rw-r--r--   0 root         (0) root         (0)     2369 2023-07-19 06:59:12.000000 netbluemind4-4.9.2928/netbluemind/system/api/IGlobalSettings.py
--rw-r--r--   0 root         (0) root         (0)    17153 2023-07-19 06:59:10.000000 netbluemind4-4.9.2928/netbluemind/system/api/IInstallation.py
--rw-r--r--   0 root         (0) root         (0)     1530 2023-07-19 06:59:09.000000 netbluemind4-4.9.2928/netbluemind/system/api/IMailDeliveryMgmt.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-07-19 06:59:09.000000 netbluemind4-4.9.2928/netbluemind/system/api/ISchemaMgmt.py
--rw-r--r--   0 root         (0) root         (0)     4029 2023-07-19 06:59:11.000000 netbluemind4-4.9.2928/netbluemind/system/api/ISecurityMgmt.py
--rw-r--r--   0 root         (0) root         (0)     2092 2023-07-19 06:59:11.000000 netbluemind4-4.9.2928/netbluemind/system/api/ISystemConfiguration.py
--rw-r--r--   0 root         (0) root         (0)     2488 2023-07-19 06:59:09.000000 netbluemind4-4.9.2928/netbluemind/system/api/InstallationVersion.py
--rw-r--r--   0 root         (0) root         (0)     2155 2023-07-19 06:59:09.000000 netbluemind4-4.9.2928/netbluemind/system/api/PublicInfos.py
--rw-r--r--   0 root         (0) root         (0)     1965 2023-07-19 06:59:11.000000 netbluemind4-4.9.2928/netbluemind/system/api/SchemaCheckInfo.py
--rw-r--r--   0 root         (0) root         (0)     7282 2023-07-19 06:59:09.000000 netbluemind4-4.9.2928/netbluemind/system/api/SubscriptionInformations.py
--rw-r--r--   0 root         (0) root         (0)     3048 2023-07-19 06:59:09.000000 netbluemind4-4.9.2928/netbluemind/system/api/SubscriptionInformationsInstallationIndicator.py
--rw-r--r--   0 root         (0) root         (0)     1266 2023-07-19 06:59:11.000000 netbluemind4-4.9.2928/netbluemind/system/api/SubscriptionInformationsInstallationIndicatorKind.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-07-19 06:59:12.000000 netbluemind4-4.9.2928/netbluemind/system/api/SubscriptionInformationsKind.py
--rw-r--r--   0 root         (0) root         (0)     3108 2023-07-19 06:59:11.000000 netbluemind4-4.9.2928/netbluemind/system/api/SubscriptionInformationsMessage.py
--rw-r--r--   0 root         (0) root         (0)     1248 2023-07-19 06:59:11.000000 netbluemind4-4.9.2928/netbluemind/system/api/SubscriptionInformationsMessageCode.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-07-19 06:59:11.000000 netbluemind4-4.9.2928/netbluemind/system/api/SubscriptionInformationsMessageKind.py
--rw-r--r--   0 root         (0) root         (0)     1555 2023-07-19 06:59:10.000000 netbluemind4-4.9.2928/netbluemind/system/api/SystemConf.py
--rw-r--r--   0 root         (0) root         (0)     1492 2023-07-19 06:59:09.000000 netbluemind4-4.9.2928/netbluemind/system/api/SystemState.py
--rw-r--r--   0 root         (0) root         (0)     2684 2023-07-19 06:59:11.000000 netbluemind4-4.9.2928/netbluemind/system/api/UpgradeReport.py
--rw-r--r--   0 root         (0) root         (0)     1114 2023-07-19 06:59:11.000000 netbluemind4-4.9.2928/netbluemind/system/api/UpgradeReportStatus.py
--rw-r--r--   0 root         (0) root         (0)     1945 2023-07-19 06:59:11.000000 netbluemind4-4.9.2928/netbluemind/system/api/UpgradeReportUpgraderReport.py
--rw-r--r--   0 root         (0) root         (0)     2115 2023-07-19 06:59:09.000000 netbluemind4-4.9.2928/netbluemind/system/api/UpgradeStatus.py
--rw-r--r--   0 root         (0) root         (0)     1199 2023-07-19 06:59:11.000000 netbluemind4-4.9.2928/netbluemind/system/api/UpgradeStatusState.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:10.000000 netbluemind4-4.9.2928/netbluemind/system/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.359159 netbluemind4-4.9.2928/netbluemind/system/api/hot/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:10.000000 netbluemind4-4.9.2928/netbluemind/system/api/hot/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.363159 netbluemind4-4.9.2928/netbluemind/system/api/hot/upgrade/
--rw-r--r--   0 root         (0) root         (0)     2466 2023-07-19 06:59:12.000000 netbluemind4-4.9.2928/netbluemind/system/api/hot/upgrade/HotUpgradeProgress.py
--rw-r--r--   0 root         (0) root         (0)     5047 2023-07-19 06:59:12.000000 netbluemind4-4.9.2928/netbluemind/system/api/hot/upgrade/HotUpgradeTask.py
--rw-r--r--   0 root         (0) root         (0)     1140 2023-07-19 06:59:12.000000 netbluemind4-4.9.2928/netbluemind/system/api/hot/upgrade/HotUpgradeTaskExecutionMode.py
--rw-r--r--   0 root         (0) root         (0)     1563 2023-07-19 06:59:12.000000 netbluemind4-4.9.2928/netbluemind/system/api/hot/upgrade/HotUpgradeTaskFilter.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-07-19 06:59:12.000000 netbluemind4-4.9.2928/netbluemind/system/api/hot/upgrade/HotUpgradeTaskStatus.py
--rw-r--r--   0 root         (0) root         (0)     3211 2023-07-19 06:59:12.000000 netbluemind4-4.9.2928/netbluemind/system/api/hot/upgrade/IHotUpgrade.py
--rw-r--r--   0 root         (0) root         (0)     5213 2023-07-19 06:59:12.000000 netbluemind4-4.9.2928/netbluemind/system/api/hot/upgrade/IInternalHotUpgrade.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:10.000000 netbluemind4-4.9.2928/netbluemind/system/api/hot/upgrade/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.363159 netbluemind4-4.9.2928/netbluemind/tag/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:10.000000 netbluemind4-4.9.2928/netbluemind/tag/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.363159 netbluemind4-4.9.2928/netbluemind/tag/api/
--rw-r--r--   0 root         (0) root         (0)     1423 2023-07-19 06:58:54.000000 netbluemind4-4.9.2928/netbluemind/tag/api/ITagUids.py
--rw-r--r--   0 root         (0) root         (0)     7936 2023-07-19 06:58:53.000000 netbluemind4-4.9.2928/netbluemind/tag/api/ITags.py
--rw-r--r--   0 root         (0) root         (0)     1689 2023-07-19 06:58:53.000000 netbluemind4-4.9.2928/netbluemind/tag/api/Tag.py
--rw-r--r--   0 root         (0) root         (0)     3243 2023-07-19 06:58:53.000000 netbluemind4-4.9.2928/netbluemind/tag/api/TagChanges.py
--rw-r--r--   0 root         (0) root         (0)     1929 2023-07-19 06:58:53.000000 netbluemind4-4.9.2928/netbluemind/tag/api/TagChangesItemAdd.py
--rw-r--r--   0 root         (0) root         (0)     1509 2023-07-19 06:58:53.000000 netbluemind4-4.9.2928/netbluemind/tag/api/TagChangesItemDelete.py
--rw-r--r--   0 root         (0) root         (0)     1938 2023-07-19 06:58:53.000000 netbluemind4-4.9.2928/netbluemind/tag/api/TagChangesItemModify.py
--rw-r--r--   0 root         (0) root         (0)     2205 2023-07-19 06:58:53.000000 netbluemind4-4.9.2928/netbluemind/tag/api/TagRef.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:10.000000 netbluemind4-4.9.2928/netbluemind/tag/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.363159 netbluemind4-4.9.2928/netbluemind/todolist/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:10.000000 netbluemind4-4.9.2928/netbluemind/todolist/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.367159 netbluemind4-4.9.2928/netbluemind/todolist/api/
--rw-r--r--   0 root         (0) root         (0)    21899 2023-07-19 06:58:55.000000 netbluemind4-4.9.2928/netbluemind/todolist/api/ITodoList.py
--rw-r--r--   0 root         (0) root         (0)     3303 2023-07-19 06:58:54.000000 netbluemind4-4.9.2928/netbluemind/todolist/api/ITodoLists.py
--rw-r--r--   0 root         (0) root         (0)     2196 2023-07-19 06:58:56.000000 netbluemind4-4.9.2928/netbluemind/todolist/api/ITodoListsMgmt.py
--rw-r--r--   0 root         (0) root         (0)     1957 2023-07-19 06:58:55.000000 netbluemind4-4.9.2928/netbluemind/todolist/api/ITodoUids.py
--rw-r--r--   0 root         (0) root         (0)     2634 2023-07-19 06:58:54.000000 netbluemind4-4.9.2928/netbluemind/todolist/api/IVTodo.py
--rw-r--r--   0 root         (0) root         (0)     2410 2023-07-19 06:58:55.000000 netbluemind4-4.9.2928/netbluemind/todolist/api/TodoListsVTodoQuery.py
--rw-r--r--   0 root         (0) root         (0)     3104 2023-07-19 06:58:54.000000 netbluemind4-4.9.2928/netbluemind/todolist/api/VTodo.py
--rw-r--r--   0 root         (0) root         (0)     3369 2023-07-19 06:58:55.000000 netbluemind4-4.9.2928/netbluemind/todolist/api/VTodoChanges.py
--rw-r--r--   0 root         (0) root         (0)     2302 2023-07-19 06:58:54.000000 netbluemind4-4.9.2928/netbluemind/todolist/api/VTodoChangesItemAdd.py
--rw-r--r--   0 root         (0) root         (0)     1842 2023-07-19 06:58:54.000000 netbluemind4-4.9.2928/netbluemind/todolist/api/VTodoChangesItemDelete.py
--rw-r--r--   0 root         (0) root         (0)     2538 2023-07-19 06:58:54.000000 netbluemind4-4.9.2928/netbluemind/todolist/api/VTodoChangesItemModify.py
--rw-r--r--   0 root         (0) root         (0)     3482 2023-07-19 06:58:54.000000 netbluemind4-4.9.2928/netbluemind/todolist/api/VTodoQuery.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:10.000000 netbluemind4-4.9.2928/netbluemind/todolist/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.367159 netbluemind4-4.9.2928/netbluemind/user/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:10.000000 netbluemind4-4.9.2928/netbluemind/user/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.371159 netbluemind4-4.9.2928/netbluemind/user/api/
--rw-r--r--   0 root         (0) root         (0)     1879 2023-07-19 06:59:00.000000 netbluemind4-4.9.2928/netbluemind/user/api/ChangePassword.py
--rw-r--r--   0 root         (0) root         (0)    16565 2023-07-19 06:59:01.000000 netbluemind4-4.9.2928/netbluemind/user/api/IUser.py
--rw-r--r--   0 root         (0) root         (0)     4869 2023-07-19 06:59:02.000000 netbluemind4-4.9.2928/netbluemind/user/api/IUserExternalAccount.py
--rw-r--r--   0 root         (0) root         (0)     5750 2023-07-19 06:59:01.000000 netbluemind4-4.9.2928/netbluemind/user/api/IUserMailIdentities.py
--rw-r--r--   0 root         (0) root         (0)     3402 2023-07-19 06:59:02.000000 netbluemind4-4.9.2928/netbluemind/user/api/IUserSettings.py
--rw-r--r--   0 root         (0) root         (0)     3990 2023-07-19 06:59:01.000000 netbluemind4-4.9.2928/netbluemind/user/api/IUserSubscription.py
--rw-r--r--   0 root         (0) root         (0)     5804 2023-07-19 06:59:00.000000 netbluemind4-4.9.2928/netbluemind/user/api/User.py
--rw-r--r--   0 root         (0) root         (0)     2159 2023-07-19 06:59:01.000000 netbluemind4-4.9.2928/netbluemind/user/api/UserAccount.py
--rw-r--r--   0 root         (0) root         (0)     1925 2023-07-19 06:59:00.000000 netbluemind4-4.9.2928/netbluemind/user/api/UserAccountInfo.py
--rw-r--r--   0 root         (0) root         (0)     1861 2023-07-19 06:59:02.000000 netbluemind4-4.9.2928/netbluemind/user/api/UserMailIdentity.py
--rw-r--r--   0 root         (0) root         (0)     1561 2023-07-19 06:59:00.000000 netbluemind4-4.9.2928/netbluemind/user/api/UserSettings.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:10.000000 netbluemind4-4.9.2928/netbluemind/user/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.371159 netbluemind4-4.9.2928/netbluemind/webappdata/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:10.000000 netbluemind4-4.9.2928/netbluemind/webappdata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.371159 netbluemind4-4.9.2928/netbluemind/webappdata/api/
--rw-r--r--   0 root         (0) root         (0)    13653 2023-07-19 06:58:50.000000 netbluemind4-4.9.2928/netbluemind/webappdata/api/IWebAppData.py
--rw-r--r--   0 root         (0) root         (0)     1464 2023-07-19 06:58:50.000000 netbluemind4-4.9.2928/netbluemind/webappdata/api/IWebAppDataUids.py
--rw-r--r--   0 root         (0) root         (0)     1692 2023-07-19 06:58:50.000000 netbluemind4-4.9.2928/netbluemind/webappdata/api/WebAppData.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 01:01:10.000000 netbluemind4-4.9.2928/netbluemind/webappdata/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:59:15.371159 netbluemind4-4.9.2928/netbluemind4.egg-info/
--rw-r--r--   0 root         (0) root         (0)      534 2023-07-19 06:59:15.000000 netbluemind4-4.9.2928/netbluemind4.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    24380 2023-07-19 06:59:15.000000 netbluemind4-4.9.2928/netbluemind4.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 06:59:15.000000 netbluemind4-4.9.2928/netbluemind4.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-19 06:59:15.000000 netbluemind4-4.9.2928/netbluemind4.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-19 06:59:15.000000 netbluemind4-4.9.2928/netbluemind4.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-07-19 06:59:15.375159 netbluemind4-4.9.2928/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      813 2023-07-19 06:59:14.000000 netbluemind4-4.9.2928/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.661647 netbluemind4-4.9.2940/
+-rw-r--r--   0 root         (0) root         (0)     2232 2023-07-27 13:47:41.000000 netbluemind4-4.9.2940/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      534 2023-07-27 13:48:42.661647 netbluemind4-4.9.2940/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      461 2023-07-27 13:47:41.000000 netbluemind4-4.9.2940/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.541644 netbluemind4-4.9.2940/netbluemind/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:14.000000 netbluemind4-4.9.2940/netbluemind/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.545644 netbluemind4-4.9.2940/netbluemind/addressbook/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:06.000000 netbluemind4-4.9.2940/netbluemind/addressbook/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.549644 netbluemind4-4.9.2940/netbluemind/addressbook/api/
+-rw-r--r--   0 root         (0) root         (0)     3021 2023-07-27 13:48:33.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/AddressBookDescriptor.py
+-rw-r--r--   0 root         (0) root         (0)    24796 2023-07-27 13:48:32.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/IAddressBook.py
+-rw-r--r--   0 root         (0) root         (0)     3064 2023-07-27 13:48:33.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/IAddressBookUids.py
+-rw-r--r--   0 root         (0) root         (0)     2156 2023-07-27 13:48:31.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/IAddressBooks.py
+-rw-r--r--   0 root         (0) root         (0)     7034 2023-07-27 13:48:30.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/IAddressBooksMgmt.py
+-rw-r--r--   0 root         (0) root         (0)     2734 2023-07-27 13:48:30.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/IVCardService.py
+-rw-r--r--   0 root         (0) root         (0)     6805 2023-07-27 13:48:33.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCard.py
+-rw-r--r--   0 root         (0) root         (0)     2204 2023-07-27 13:48:31.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardBasicAttribute.py
+-rw-r--r--   0 root         (0) root         (0)     3405 2023-07-27 13:48:31.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardChanges.py
+-rw-r--r--   0 root         (0) root         (0)     2218 2023-07-27 13:48:30.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardChangesItemAdd.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-07-27 13:48:30.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardChangesItemDelete.py
+-rw-r--r--   0 root         (0) root         (0)     2227 2023-07-27 13:48:31.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardChangesItemModify.py
+-rw-r--r--   0 root         (0) root         (0)     4211 2023-07-27 13:48:30.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardCommunications.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2023-07-27 13:48:30.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardCommunicationsEmail.py
+-rw-r--r--   0 root         (0) root         (0)     1702 2023-07-27 13:48:31.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardCommunicationsImpp.py
+-rw-r--r--   0 root         (0) root         (0)     1702 2023-07-27 13:48:31.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardCommunicationsLang.py
+-rw-r--r--   0 root         (0) root         (0)     1894 2023-07-27 13:48:31.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardCommunicationsTel.py
+-rw-r--r--   0 root         (0) root         (0)     2085 2023-07-27 13:48:31.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardDeliveryAddressing.py
+-rw-r--r--   0 root         (0) root         (0)     3596 2023-07-27 13:48:33.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardDeliveryAddressingAddress.py
+-rw-r--r--   0 root         (0) root         (0)     2750 2023-07-27 13:48:31.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardExplanatory.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2023-07-27 13:48:32.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardExplanatoryUrl.py
+-rw-r--r--   0 root         (0) root         (0)     5236 2023-07-27 13:48:33.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardIdentification.py
+-rw-r--r--   0 root         (0) root         (0)     1726 2023-07-27 13:48:30.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardIdentificationFormatedName.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-07-27 13:48:33.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardIdentificationGender.py
+-rw-r--r--   0 root         (0) root         (0)     3023 2023-07-27 13:48:32.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardIdentificationName.py
+-rw-r--r--   0 root         (0) root         (0)     1714 2023-07-27 13:48:30.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardIdentificationNickname.py
+-rw-r--r--   0 root         (0) root         (0)     3734 2023-07-27 13:48:33.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardInfo.py
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-07-27 13:48:30.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardKind.py
+-rw-r--r--   0 root         (0) root         (0)     3115 2023-07-27 13:48:31.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardOrganizational.py
+-rw-r--r--   0 root         (0) root         (0)     2316 2023-07-27 13:48:33.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardOrganizationalMember.py
+-rw-r--r--   0 root         (0) root         (0)     2049 2023-07-27 13:48:33.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardOrganizationalOrg.py
+-rw-r--r--   0 root         (0) root         (0)     1722 2023-07-27 13:48:32.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardParameter.py
+-rw-r--r--   0 root         (0) root         (0)     2788 2023-07-27 13:48:31.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardQuery.py
+-rw-r--r--   0 root         (0) root         (0)     1136 2023-07-27 13:48:30.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardQueryOrderBy.py
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-07-27 13:48:33.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardRelated.py
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-07-27 13:48:31.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardSecurity.py
+-rw-r--r--   0 root         (0) root         (0)     1681 2023-07-27 13:48:32.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardSecurityKey.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:06.000000 netbluemind4-4.9.2940/netbluemind/addressbook/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.553644 netbluemind4-4.9.2940/netbluemind/attachment/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:12.000000 netbluemind4-4.9.2940/netbluemind/attachment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.553644 netbluemind4-4.9.2940/netbluemind/attachment/api/
+-rw-r--r--   0 root         (0) root         (0)     2228 2023-07-27 13:47:52.000000 netbluemind4-4.9.2940/netbluemind/attachment/api/AttachedFile.py
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-07-27 13:47:52.000000 netbluemind4-4.9.2940/netbluemind/attachment/api/Configuration.py
+-rw-r--r--   0 root         (0) root         (0)     3699 2023-07-27 13:47:53.000000 netbluemind4-4.9.2940/netbluemind/attachment/api/IAttachment.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:12.000000 netbluemind4-4.9.2940/netbluemind/attachment/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.553644 netbluemind4-4.9.2940/netbluemind/authentication/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:06.000000 netbluemind4-4.9.2940/netbluemind/authentication/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.553644 netbluemind4-4.9.2940/netbluemind/authentication/api/
+-rw-r--r--   0 root         (0) root         (0)     2214 2023-07-27 13:48:36.000000 netbluemind4-4.9.2940/netbluemind/authentication/api/APIKey.py
+-rw-r--r--   0 root         (0) root         (0)     4622 2023-07-27 13:48:35.000000 netbluemind4-4.9.2940/netbluemind/authentication/api/AccessTokenInfo.py
+-rw-r--r--   0 root         (0) root         (0)     1205 2023-07-27 13:48:35.000000 netbluemind4-4.9.2940/netbluemind/authentication/api/AccessTokenInfoTokenStatus.py
+-rw-r--r--   0 root         (0) root         (0)     3330 2023-07-27 13:48:35.000000 netbluemind4-4.9.2940/netbluemind/authentication/api/AuthUser.py
+-rw-r--r--   0 root         (0) root         (0)     3891 2023-07-27 13:48:35.000000 netbluemind4-4.9.2940/netbluemind/authentication/api/IAPIKeys.py
+-rw-r--r--   0 root         (0) root         (0)     6122 2023-07-27 13:48:36.000000 netbluemind4-4.9.2940/netbluemind/authentication/api/IAuthentication.py
+-rw-r--r--   0 root         (0) root         (0)     2400 2023-07-27 13:48:35.000000 netbluemind4-4.9.2940/netbluemind/authentication/api/ISecurityToken.py
+-rw-r--r--   0 root         (0) root         (0)     1387 2023-07-27 13:48:36.000000 netbluemind4-4.9.2940/netbluemind/authentication/api/ISudoSupport.py
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-07-27 13:48:35.000000 netbluemind4-4.9.2940/netbluemind/authentication/api/IUserAccessToken.py
+-rw-r--r--   0 root         (0) root         (0)     3151 2023-07-27 13:48:35.000000 netbluemind4-4.9.2940/netbluemind/authentication/api/LoginResponse.py
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-07-27 13:48:35.000000 netbluemind4-4.9.2940/netbluemind/authentication/api/LoginResponseStatus.py
+-rw-r--r--   0 root         (0) root         (0)     1167 2023-07-27 13:48:35.000000 netbluemind4-4.9.2940/netbluemind/authentication/api/ValidationKind.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:06.000000 netbluemind4-4.9.2940/netbluemind/authentication/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.553644 netbluemind4-4.9.2940/netbluemind/backend/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:08.000000 netbluemind4-4.9.2940/netbluemind/backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.557644 netbluemind4-4.9.2940/netbluemind/backend/mail/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:08.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.565644 netbluemind4-4.9.2940/netbluemind/backend/mail/api/
+-rw-r--r--   0 root         (0) root         (0)     2063 2023-07-27 13:47:59.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/Conversation.py
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-07-27 13:48:00.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/ConversationMessageRef.py
+-rw-r--r--   0 root         (0) root         (0)     1118 2023-07-27 13:48:00.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/DispositionType.py
+-rw-r--r--   0 root         (0) root         (0)    10560 2023-07-27 13:48:04.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/IBaseMailboxFolders.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2023-07-27 13:47:59.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/IItemsTransfer.py
+-rw-r--r--   0 root         (0) root         (0)     4309 2023-07-27 13:48:05.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/IMailConversation.py
+-rw-r--r--   0 root         (0) root         (0)     6827 2023-07-27 13:48:00.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/IMailConversationActions.py
+-rw-r--r--   0 root         (0) root         (0)    19004 2023-07-27 13:48:02.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/IMailboxFolders.py
+-rw-r--r--   0 root         (0) root         (0)    19154 2023-07-27 13:48:00.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/IMailboxFoldersByContainer.py
+-rw-r--r--   0 root         (0) root         (0)    21454 2023-07-27 13:48:03.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/IMailboxItems.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2023-07-27 13:48:02.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/IOutbox.py
+-rw-r--r--   0 root         (0) root         (0)    10771 2023-07-27 13:48:05.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/IReadOnlyMailboxFolders.py
+-rw-r--r--   0 root         (0) root         (0)     1579 2023-07-27 13:47:59.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/IUserInbox.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2023-07-27 13:48:03.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/ImapAck.py
+-rw-r--r--   0 root         (0) root         (0)     1884 2023-07-27 13:47:59.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/ImapItemIdentifier.py
+-rw-r--r--   0 root         (0) root         (0)     3634 2023-07-27 13:47:59.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/ImportMailboxItemSet.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-07-27 13:48:05.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/ImportMailboxItemSetMailboxItemId.py
+-rw-r--r--   0 root         (0) root         (0)     3090 2023-07-27 13:48:02.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/ImportMailboxItemsStatus.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-07-27 13:48:02.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/ImportMailboxItemsStatusImportStatus.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-07-27 13:48:05.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/ImportMailboxItemsStatusImportedMailboxItem.py
+-rw-r--r--   0 root         (0) root         (0)     2219 2023-07-27 13:48:03.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/MailboxFolder.py
+-rw-r--r--   0 root         (0) root         (0)     2397 2023-07-27 13:48:03.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/MailboxFolderSearchQuery.py
+-rw-r--r--   0 root         (0) root         (0)     2723 2023-07-27 13:47:59.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/MailboxItem.py
+-rw-r--r--   0 root         (0) root         (0)     5517 2023-07-27 13:48:01.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/MessageBody.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-07-27 13:47:59.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/MessageBodyHeader.py
+-rw-r--r--   0 root         (0) root         (0)     4943 2023-07-27 13:48:02.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/MessageBodyPart.py
+-rw-r--r--   0 root         (0) root         (0)     2397 2023-07-27 13:48:02.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/MessageBodyRecipient.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2023-07-27 13:48:05.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/MessageBodyRecipientKind.py
+-rw-r--r--   0 root         (0) root         (0)     4966 2023-07-27 13:48:04.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/MessageSearchResult.py
+-rw-r--r--   0 root         (0) root         (0)     2088 2023-07-27 13:48:01.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/MessageSearchResultMbox.py
+-rw-r--r--   0 root         (0) root         (0)     5250 2023-07-27 13:48:01.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/SearchQuery.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-07-27 13:48:00.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/SearchQueryFolderScope.py
+-rw-r--r--   0 root         (0) root         (0)     1722 2023-07-27 13:48:02.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/SearchQueryHeader.py
+-rw-r--r--   0 root         (0) root         (0)     2800 2023-07-27 13:48:02.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/SearchQueryHeaderQuery.py
+-rw-r--r--   0 root         (0) root         (0)     1129 2023-07-27 13:47:59.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/SearchQueryLogicalOperator.py
+-rw-r--r--   0 root         (0) root         (0)     2360 2023-07-27 13:48:03.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/SearchQuerySearchScope.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2023-07-27 13:48:00.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/SearchResult.py
+-rw-r--r--   0 root         (0) root         (0)     2030 2023-07-27 13:48:01.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/SearchSort.py
+-rw-r--r--   0 root         (0) root         (0)     1100 2023-07-27 13:48:00.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/SearchSortOrder.py
+-rw-r--r--   0 root         (0) root         (0)     2118 2023-07-27 13:48:02.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/SearchSortSortCriteria.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:08.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.565644 netbluemind4-4.9.2940/netbluemind/backend/mail/api/flags/
+-rw-r--r--   0 root         (0) root         (0)     2408 2023-07-27 13:48:05.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/flags/ConversationFlagUpdate.py
+-rw-r--r--   0 root         (0) root         (0)     2274 2023-07-27 13:48:05.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/flags/FlagUpdate.py
+-rw-r--r--   0 root         (0) root         (0)     2340 2023-07-27 13:48:05.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/flags/ImportMailboxConversationSet.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-07-27 13:48:05.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/flags/MailboxItemFlag.py
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-07-27 13:48:05.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/flags/MailboxItemFlagSystem.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:08.000000 netbluemind4-4.9.2940/netbluemind/backend/mail/api/flags/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.565644 netbluemind4-4.9.2940/netbluemind/calendar/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:08.000000 netbluemind4-4.9.2940/netbluemind/calendar/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.577645 netbluemind4-4.9.2940/netbluemind/calendar/api/
+-rw-r--r--   0 root         (0) root         (0)     2788 2023-07-27 13:47:53.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/CalendarDescriptor.py
+-rw-r--r--   0 root         (0) root         (0)     3116 2023-07-27 13:47:54.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/CalendarLookupResponse.py
+-rw-r--r--   0 root         (0) root         (0)     1145 2023-07-27 13:47:54.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/CalendarLookupResponseType.py
+-rw-r--r--   0 root         (0) root         (0)     3050 2023-07-27 13:47:55.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/CalendarSettingsData.py
+-rw-r--r--   0 root         (0) root         (0)     1188 2023-07-27 13:47:53.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/CalendarSettingsDataDay.py
+-rw-r--r--   0 root         (0) root         (0)     2770 2023-07-27 13:47:54.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/CalendarView.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-07-27 13:47:53.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/CalendarViewCalendarViewType.py
+-rw-r--r--   0 root         (0) root         (0)     3600 2023-07-27 13:47:55.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/CalendarViewChanges.py
+-rw-r--r--   0 root         (0) root         (0)     2066 2023-07-27 13:47:54.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/CalendarViewChangesItemAdd.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-07-27 13:47:54.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/CalendarViewChangesItemDelete.py
+-rw-r--r--   0 root         (0) root         (0)     2075 2023-07-27 13:47:54.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/CalendarViewChangesItemModify.py
+-rw-r--r--   0 root         (0) root         (0)     2436 2023-07-27 13:47:55.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/CalendarsVEventQuery.py
+-rw-r--r--   0 root         (0) root         (0)    24195 2023-07-27 13:47:57.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/ICalendar.py
+-rw-r--r--   0 root         (0) root         (0)     2750 2023-07-27 13:47:55.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/ICalendarAutocomplete.py
+-rw-r--r--   0 root         (0) root         (0)     2440 2023-07-27 13:47:54.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/ICalendarSettings.py
+-rw-r--r--   0 root         (0) root         (0)     2496 2023-07-27 13:47:59.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/ICalendarUids.py
+-rw-r--r--   0 root         (0) root         (0)     6957 2023-07-27 13:47:57.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/ICalendarView.py
+-rw-r--r--   0 root         (0) root         (0)     1467 2023-07-27 13:47:55.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/ICalendarViewUids.py
+-rw-r--r--   0 root         (0) root         (0)     3049 2023-07-27 13:47:55.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/ICalendars.py
+-rw-r--r--   0 root         (0) root         (0)     4943 2023-07-27 13:47:58.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/ICalendarsMgmt.py
+-rw-r--r--   0 root         (0) root         (0)     3067 2023-07-27 13:47:58.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/IFreebusyMgmt.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-07-27 13:47:58.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/IFreebusyUids.py
+-rw-r--r--   0 root         (0) root         (0)     1752 2023-07-27 13:47:58.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/IPrint.py
+-rw-r--r--   0 root         (0) root         (0)     3473 2023-07-27 13:47:58.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/IPublicFreebusy.py
+-rw-r--r--   0 root         (0) root         (0)     3665 2023-07-27 13:47:55.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/IPublishCalendar.py
+-rw-r--r--   0 root         (0) root         (0)    14235 2023-07-27 13:47:54.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/IUserCalendarViews.py
+-rw-r--r--   0 root         (0) root         (0)     2596 2023-07-27 13:47:54.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/IVEvent.py
+-rw-r--r--   0 root         (0) root         (0)     2623 2023-07-27 13:47:58.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/IVFreebusy.py
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-07-27 13:47:57.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/PrintData.py
+-rw-r--r--   0 root         (0) root         (0)     5946 2023-07-27 13:47:54.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/PrintOptions.py
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-07-27 13:47:55.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/PrintOptionsCalendarMetadata.py
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-07-27 13:47:55.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/PrintOptionsPrintFormat.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-07-27 13:47:54.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/PrintOptionsPrintLayout.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-07-27 13:47:54.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/PrintOptionsPrintView.py
+-rw-r--r--   0 root         (0) root         (0)     1100 2023-07-27 13:47:58.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/PublishMode.py
+-rw-r--r--   0 root         (0) root         (0)     2821 2023-07-27 13:47:55.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/VEvent.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2023-07-27 13:47:53.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/VEventAttendeeQuery.py
+-rw-r--r--   0 root         (0) root         (0)     3402 2023-07-27 13:47:55.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/VEventChanges.py
+-rw-r--r--   0 root         (0) root         (0)     2375 2023-07-27 13:47:58.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/VEventChangesItemAdd.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2023-07-27 13:47:54.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/VEventChangesItemDelete.py
+-rw-r--r--   0 root         (0) root         (0)     2384 2023-07-27 13:47:57.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/VEventChangesItemModify.py
+-rw-r--r--   0 root         (0) root         (0)     2667 2023-07-27 13:47:58.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/VEventCounter.py
+-rw-r--r--   0 root         (0) root         (0)     1815 2023-07-27 13:47:54.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/VEventCounterCounterOriginator.py
+-rw-r--r--   0 root         (0) root         (0)     2112 2023-07-27 13:47:55.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/VEventOccurrence.py
+-rw-r--r--   0 root         (0) root         (0)     4230 2023-07-27 13:47:58.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/VEventQuery.py
+-rw-r--r--   0 root         (0) root         (0)     3935 2023-07-27 13:47:56.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/VEventSeries.py
+-rw-r--r--   0 root         (0) root         (0)     1129 2023-07-27 13:47:55.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/VEventTransparency.py
+-rw-r--r--   0 root         (0) root         (0)     2958 2023-07-27 13:47:57.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/VFreebusy.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2023-07-27 13:47:53.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/VFreebusyQuery.py
+-rw-r--r--   0 root         (0) root         (0)     3128 2023-07-27 13:47:55.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/VFreebusySlot.py
+-rw-r--r--   0 root         (0) root         (0)     1172 2023-07-27 13:47:53.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/VFreebusyType.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:08.000000 netbluemind4-4.9.2940/netbluemind/calendar/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.577645 netbluemind4-4.9.2940/netbluemind/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:08.000000 netbluemind4-4.9.2940/netbluemind/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.581645 netbluemind4-4.9.2940/netbluemind/core/api/
+-rw-r--r--   0 root         (0) root         (0)     2011 2023-07-27 13:48:14.000000 netbluemind4-4.9.2940/netbluemind/core/api/Email.py
+-rw-r--r--   0 root         (0) root         (0)     1736 2023-07-27 13:48:14.000000 netbluemind4-4.9.2940/netbluemind/core/api/ImportStats.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-07-27 13:48:14.000000 netbluemind4-4.9.2940/netbluemind/core/api/ListResult.py
+-rw-r--r--   0 root         (0) root         (0)     2211 2023-07-27 13:48:14.000000 netbluemind4-4.9.2940/netbluemind/core/api/VersionInfo.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:06.000000 netbluemind4-4.9.2940/netbluemind/core/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.581645 netbluemind4-4.9.2940/netbluemind/core/api/date/
+-rw-r--r--   0 root         (0) root         (0)     2417 2023-07-27 13:48:14.000000 netbluemind4-4.9.2940/netbluemind/core/api/date/BmDateTime.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-07-27 13:48:14.000000 netbluemind4-4.9.2940/netbluemind/core/api/date/BmDateTimePrecision.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:06.000000 netbluemind4-4.9.2940/netbluemind/core/api/date/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.581645 netbluemind4-4.9.2940/netbluemind/core/api/fault/
+-rw-r--r--   0 root         (0) root         (0)     5090 2023-07-27 13:48:14.000000 netbluemind4-4.9.2940/netbluemind/core/api/fault/ErrorCode.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:06.000000 netbluemind4-4.9.2940/netbluemind/core/api/fault/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.581645 netbluemind4-4.9.2940/netbluemind/core/container/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:08.000000 netbluemind4-4.9.2940/netbluemind/core/container/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.585645 netbluemind4-4.9.2940/netbluemind/core/container/api/
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-07-27 13:48:11.000000 netbluemind4-4.9.2940/netbluemind/core/container/api/Ack.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-07-27 13:48:10.000000 netbluemind4-4.9.2940/netbluemind/core/container/api/ContainerHierarchyNode.py
+-rw-r--r--   0 root         (0) root         (0)     2906 2023-07-27 13:48:12.000000 netbluemind4-4.9.2940/netbluemind/core/container/api/ContainerQuery.py
+-rw-r--r--   0 root         (0) root         (0)     1862 2023-07-27 13:48:10.000000 netbluemind4-4.9.2940/netbluemind/core/container/api/ContainerSubscription.py
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-07-27 13:48:11.000000 netbluemind4-4.9.2940/netbluemind/core/container/api/ContainerSubscriptionDescriptor.py
+-rw-r--r--   0 root         (0) root         (0)     2762 2023-07-27 13:48:11.000000 netbluemind4-4.9.2940/netbluemind/core/container/api/ContainerSubscriptionModel.py
+-rw-r--r--   0 root         (0) root         (0)     1478 2023-07-27 13:48:12.000000 netbluemind4-4.9.2940/netbluemind/core/container/api/Count.py
+-rw-r--r--   0 root         (0) root         (0)     6266 2023-07-27 13:48:12.000000 netbluemind4-4.9.2940/netbluemind/core/container/api/IChangelogSupport.py
+-rw-r--r--   0 root         (0) root         (0)    10791 2023-07-27 13:48:12.000000 netbluemind4-4.9.2940/netbluemind/core/container/api/IContainerManagement.py
+-rw-r--r--   0 root         (0) root         (0)     2974 2023-07-27 13:48:12.000000 netbluemind4-4.9.2940/netbluemind/core/container/api/IContainerSync.py
+-rw-r--r--   0 root         (0) root         (0)    10675 2023-07-27 13:48:11.000000 netbluemind4-4.9.2940/netbluemind/core/container/api/IContainers.py
+-rw-r--r--   0 root         (0) root         (0)    10290 2023-07-27 13:48:13.000000 netbluemind4-4.9.2940/netbluemind/core/container/api/IContainersFlatHierarchy.py
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-07-27 13:48:14.000000 netbluemind4-4.9.2940/netbluemind/core/container/api/ICountingSupport.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-07-27 13:48:13.000000 netbluemind4-4.9.2940/netbluemind/core/container/api/IFlatHierarchyUids.py
+-rw-r--r--   0 root         (0) root         (0)     1799 2023-07-27 13:48:11.000000 netbluemind4-4.9.2940/netbluemind/core/container/api/IOfflineMgmt.py
+-rw-r--r--   0 root         (0) root         (0)     1543 2023-07-27 13:48:10.000000 netbluemind4-4.9.2940/netbluemind/core/container/api/IOwnerSubscriptionUids.py
+-rw-r--r--   0 root         (0) root         (0)    12217 2023-07-27 13:48:14.000000 netbluemind4-4.9.2940/netbluemind/core/container/api/IOwnerSubscriptions.py
+-rw-r--r--   0 root         (0) root         (0)     1667 2023-07-27 13:48:10.000000 netbluemind4-4.9.2940/netbluemind/core/container/api/ISortingSupport.py
+-rw-r--r--   0 root         (0) root         (0)     1763 2023-07-27 13:48:10.000000 netbluemind4-4.9.2940/netbluemind/core/container/api/IdRange.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:08.000000 netbluemind4-4.9.2940/netbluemind/core/container/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.589645 netbluemind4-4.9.2940/netbluemind/core/container/model/
+-rw-r--r--   0 root         (0) root         (0)     4440 2023-07-27 13:48:09.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/BaseContainerDescriptor.py
+-rw-r--r--   0 root         (0) root         (0)     3777 2023-07-27 13:48:10.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/ChangeLogEntry.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2023-07-27 13:48:10.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/ChangeLogEntryType.py
+-rw-r--r--   0 root         (0) root         (0)     1981 2023-07-27 13:48:10.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/ContainerChangelog.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-07-27 13:48:10.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/ContainerChangeset.py
+-rw-r--r--   0 root         (0) root         (0)     3053 2023-07-27 13:48:10.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/ContainerDescriptor.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-07-27 13:48:10.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/ContainerModifiableDescriptor.py
+-rw-r--r--   0 root         (0) root         (0)     2861 2023-07-27 13:48:09.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/ContainerSyncResult.py
+-rw-r--r--   0 root         (0) root         (0)     3156 2023-07-27 13:48:09.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/ContainerSyncStatus.py
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-07-27 13:48:09.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/ContainerSyncStatusStatus.py
+-rw-r--r--   0 root         (0) root         (0)     3489 2023-07-27 13:48:09.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/ContainerUpdatesResult.py
+-rw-r--r--   0 root         (0) root         (0)     2320 2023-07-27 13:48:10.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/ContainerUpdatesResultInError.py
+-rw-r--r--   0 root         (0) root         (0)     2677 2023-07-27 13:48:09.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/IdQuery.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-07-27 13:48:10.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/ItemChangeLogEntry.py
+-rw-r--r--   0 root         (0) root         (0)     2006 2023-07-27 13:48:09.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/ItemChangelog.py
+-rw-r--r--   0 root         (0) root         (0)     3737 2023-07-27 13:48:10.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/ItemContainerValue.py
+-rw-r--r--   0 root         (0) root         (0)     4056 2023-07-27 13:48:10.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/ItemDescriptor.py
+-rw-r--r--   0 root         (0) root         (0)     1115 2023-07-27 13:48:09.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/ItemFlag.py
+-rw-r--r--   0 root         (0) root         (0)     2853 2023-07-27 13:48:10.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/ItemFlagFilter.py
+-rw-r--r--   0 root         (0) root         (0)     1816 2023-07-27 13:48:10.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/ItemIdentifier.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-07-27 13:48:10.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/ItemUri.py
+-rw-r--r--   0 root         (0) root         (0)     4295 2023-07-27 13:48:10.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/ItemValue.py
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-07-27 13:48:10.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/ItemVersion.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-07-27 13:48:10.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/SortDescriptor.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-07-27 13:48:10.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/SortDescriptorDirection.py
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-07-27 13:48:10.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/SortDescriptorField.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:08.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.589645 netbluemind4-4.9.2940/netbluemind/core/container/model/acl/
+-rw-r--r--   0 root         (0) root         (0)     2037 2023-07-27 13:48:10.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/acl/AccessControlEntry.py
+-rw-r--r--   0 root         (0) root         (0)     1199 2023-07-27 13:48:10.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/acl/Verb.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:08.000000 netbluemind4-4.9.2940/netbluemind/core/container/model/acl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.589645 netbluemind4-4.9.2940/netbluemind/core/task/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:08.000000 netbluemind4-4.9.2940/netbluemind/core/task/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.593645 netbluemind4-4.9.2940/netbluemind/core/task/api/
+-rw-r--r--   0 root         (0) root         (0)     2471 2023-07-27 13:48:14.000000 netbluemind4-4.9.2940/netbluemind/core/task/api/ITask.py
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-07-27 13:48:14.000000 netbluemind4-4.9.2940/netbluemind/core/task/api/TaskRef.py
+-rw-r--r--   0 root         (0) root         (0)     2808 2023-07-27 13:48:14.000000 netbluemind4-4.9.2940/netbluemind/core/task/api/TaskStatus.py
+-rw-r--r--   0 root         (0) root         (0)     1174 2023-07-27 13:48:14.000000 netbluemind4-4.9.2940/netbluemind/core/task/api/TaskStatusState.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:08.000000 netbluemind4-4.9.2940/netbluemind/core/task/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.593645 netbluemind4-4.9.2940/netbluemind/cti/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:08.000000 netbluemind4-4.9.2940/netbluemind/cti/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.593645 netbluemind4-4.9.2940/netbluemind/cti/api/
+-rw-r--r--   0 root         (0) root         (0)     4038 2023-07-27 13:48:14.000000 netbluemind4-4.9.2940/netbluemind/cti/api/IComputerTelephonyIntegration.py
+-rw-r--r--   0 root         (0) root         (0)     2610 2023-07-27 13:48:14.000000 netbluemind4-4.9.2940/netbluemind/cti/api/Status.py
+-rw-r--r--   0 root         (0) root         (0)     1219 2023-07-27 13:48:14.000000 netbluemind4-4.9.2940/netbluemind/cti/api/StatusPhoneState.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2023-07-27 13:48:14.000000 netbluemind4-4.9.2940/netbluemind/cti/api/StatusType.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:08.000000 netbluemind4-4.9.2940/netbluemind/cti/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.593645 netbluemind4-4.9.2940/netbluemind/dataprotect/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/dataprotect/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.593645 netbluemind4-4.9.2940/netbluemind/dataprotect/api/
+-rw-r--r--   0 root         (0) root         (0)     3500 2023-07-27 13:48:15.000000 netbluemind4-4.9.2940/netbluemind/dataprotect/api/DataProtectGeneration.py
+-rw-r--r--   0 root         (0) root         (0)     4139 2023-07-27 13:48:15.000000 netbluemind4-4.9.2940/netbluemind/dataprotect/api/GenerationContent.py
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-07-27 13:48:15.000000 netbluemind4-4.9.2940/netbluemind/dataprotect/api/GenerationStatus.py
+-rw-r--r--   0 root         (0) root         (0)     8292 2023-07-27 13:48:15.000000 netbluemind4-4.9.2940/netbluemind/dataprotect/api/IDataProtect.py
+-rw-r--r--   0 root         (0) root         (0)     4132 2023-07-27 13:48:15.000000 netbluemind4-4.9.2940/netbluemind/dataprotect/api/PartGeneration.py
+-rw-r--r--   0 root         (0) root         (0)     2878 2023-07-27 13:48:15.000000 netbluemind4-4.9.2940/netbluemind/dataprotect/api/Restorable.py
+-rw-r--r--   0 root         (0) root         (0)     1229 2023-07-27 13:48:15.000000 netbluemind4-4.9.2940/netbluemind/dataprotect/api/RestorableKind.py
+-rw-r--r--   0 root         (0) root         (0)     2507 2023-07-27 13:48:15.000000 netbluemind4-4.9.2940/netbluemind/dataprotect/api/RestoreDefinition.py
+-rw-r--r--   0 root         (0) root         (0)     2389 2023-07-27 13:48:15.000000 netbluemind4-4.9.2940/netbluemind/dataprotect/api/RestoreOperation.py
+-rw-r--r--   0 root         (0) root         (0)     1947 2023-07-27 13:48:15.000000 netbluemind4-4.9.2940/netbluemind/dataprotect/api/RetentionPolicy.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/dataprotect/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.593645 netbluemind4-4.9.2940/netbluemind/device/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/device/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.597645 netbluemind4-4.9.2940/netbluemind/device/api/
+-rw-r--r--   0 root         (0) root         (0)     3871 2023-07-27 13:48:09.000000 netbluemind4-4.9.2940/netbluemind/device/api/Device.py
+-rw-r--r--   0 root         (0) root         (0)     8350 2023-07-27 13:48:09.000000 netbluemind4-4.9.2940/netbluemind/device/api/IDevice.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-07-27 13:48:09.000000 netbluemind4-4.9.2940/netbluemind/device/api/IDeviceUids.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-07-27 13:48:09.000000 netbluemind4-4.9.2940/netbluemind/device/api/IDevices.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/device/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.597645 netbluemind4-4.9.2940/netbluemind/directory/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/directory/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.601645 netbluemind4-4.9.2940/netbluemind/directory/api/
+-rw-r--r--   0 root         (0) root         (0)     3091 2023-07-27 13:48:41.000000 netbluemind4-4.9.2940/netbluemind/directory/api/BaseDirEntry.py
+-rw-r--r--   0 root         (0) root         (0)     1168 2023-07-27 13:48:41.000000 netbluemind4-4.9.2940/netbluemind/directory/api/BaseDirEntryAccountType.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-07-27 13:48:41.000000 netbluemind4-4.9.2940/netbluemind/directory/api/BaseDirEntryKind.py
+-rw-r--r--   0 root         (0) root         (0)     3052 2023-07-27 13:48:41.000000 netbluemind4-4.9.2940/netbluemind/directory/api/DirBaseValue.py
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-07-27 13:48:41.000000 netbluemind4-4.9.2940/netbluemind/directory/api/DirEntry.py
+-rw-r--r--   0 root         (0) root         (0)     7466 2023-07-27 13:48:41.000000 netbluemind4-4.9.2940/netbluemind/directory/api/DirEntryQuery.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-07-27 13:48:41.000000 netbluemind4-4.9.2940/netbluemind/directory/api/DirEntryQueryDir.py
+-rw-r--r--   0 root         (0) root         (0)     2469 2023-07-27 13:48:41.000000 netbluemind4-4.9.2940/netbluemind/directory/api/DirEntryQueryOrder.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-07-27 13:48:41.000000 netbluemind4-4.9.2940/netbluemind/directory/api/DirEntryQueryOrderBy.py
+-rw-r--r--   0 root         (0) root         (0)     1157 2023-07-27 13:48:41.000000 netbluemind4-4.9.2940/netbluemind/directory/api/DirEntryQueryStateFilter.py
+-rw-r--r--   0 root         (0) root         (0)     2719 2023-07-27 13:48:42.000000 netbluemind4-4.9.2940/netbluemind/directory/api/IDirEntryMaintenance.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2023-07-27 13:48:42.000000 netbluemind4-4.9.2940/netbluemind/directory/api/IDirEntryPath.py
+-rw-r--r--   0 root         (0) root         (0)    14188 2023-07-27 13:48:40.000000 netbluemind4-4.9.2940/netbluemind/directory/api/IDirectory.py
+-rw-r--r--   0 root         (0) root         (0)     9345 2023-07-27 13:48:42.000000 netbluemind4-4.9.2940/netbluemind/directory/api/IOrgUnits.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-07-27 13:48:41.000000 netbluemind4-4.9.2940/netbluemind/directory/api/MaintenanceOperation.py
+-rw-r--r--   0 root         (0) root         (0)     1728 2023-07-27 13:48:41.000000 netbluemind4-4.9.2940/netbluemind/directory/api/OrgUnit.py
+-rw-r--r--   0 root         (0) root         (0)     2228 2023-07-27 13:48:41.000000 netbluemind4-4.9.2940/netbluemind/directory/api/OrgUnitPath.py
+-rw-r--r--   0 root         (0) root         (0)     2632 2023-07-27 13:48:41.000000 netbluemind4-4.9.2940/netbluemind/directory/api/OrgUnitQuery.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2023-07-27 13:48:41.000000 netbluemind4-4.9.2940/netbluemind/directory/api/RepairConfig.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/directory/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.601645 netbluemind4-4.9.2940/netbluemind/document/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/document/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.601645 netbluemind4-4.9.2940/netbluemind/document/api/
+-rw-r--r--   0 root         (0) root         (0)     2146 2023-07-27 13:48:08.000000 netbluemind4-4.9.2940/netbluemind/document/api/Document.py
+-rw-r--r--   0 root         (0) root         (0)     2412 2023-07-27 13:48:08.000000 netbluemind4-4.9.2940/netbluemind/document/api/DocumentMetadata.py
+-rw-r--r--   0 root         (0) root         (0)     5027 2023-07-27 13:48:08.000000 netbluemind4-4.9.2940/netbluemind/document/api/IDocument.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/document/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.601645 netbluemind4-4.9.2940/netbluemind/documentfolder/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/documentfolder/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.601645 netbluemind4-4.9.2940/netbluemind/documentfolder/api/
+-rw-r--r--   0 root         (0) root         (0)     1695 2023-07-27 13:48:08.000000 netbluemind4-4.9.2940/netbluemind/documentfolder/api/DocumentFolder.py
+-rw-r--r--   0 root         (0) root         (0)     4166 2023-07-27 13:48:08.000000 netbluemind4-4.9.2940/netbluemind/documentfolder/api/IDocumentFolder.py
+-rw-r--r--   0 root         (0) root         (0)     1482 2023-07-27 13:48:08.000000 netbluemind4-4.9.2940/netbluemind/documentfolder/api/IDocumentFolderUids.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/documentfolder/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.605645 netbluemind4-4.9.2940/netbluemind/domain/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/domain/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.605645 netbluemind4-4.9.2940/netbluemind/domain/api/
+-rw-r--r--   0 root         (0) root         (0)     3063 2023-07-27 13:48:30.000000 netbluemind4-4.9.2940/netbluemind/domain/api/Domain.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2023-07-27 13:48:30.000000 netbluemind4-4.9.2940/netbluemind/domain/api/IDomainSettings.py
+-rw-r--r--   0 root         (0) root         (0)     8252 2023-07-27 13:48:30.000000 netbluemind4-4.9.2940/netbluemind/domain/api/IDomains.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/domain/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.605645 netbluemind4-4.9.2940/netbluemind/eas/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/eas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.605645 netbluemind4-4.9.2940/netbluemind/eas/api/
+-rw-r--r--   0 root         (0) root         (0)     1728 2023-07-27 13:48:23.000000 netbluemind4-4.9.2940/netbluemind/eas/api/Account.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2023-07-27 13:48:23.000000 netbluemind4-4.9.2940/netbluemind/eas/api/FolderSyncVersions.py
+-rw-r--r--   0 root         (0) root         (0)     1739 2023-07-27 13:48:23.000000 netbluemind4-4.9.2940/netbluemind/eas/api/Heartbeat.py
+-rw-r--r--   0 root         (0) root         (0)     7128 2023-07-27 13:48:23.000000 netbluemind4-4.9.2940/netbluemind/eas/api/IEas.py
+-rw-r--r--   0 root         (0) root         (0)     1920 2023-07-27 13:48:23.000000 netbluemind4-4.9.2940/netbluemind/eas/api/SentItem.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/eas/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.605645 netbluemind4-4.9.2940/netbluemind/externaluser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:12.000000 netbluemind4-4.9.2940/netbluemind/externaluser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.605645 netbluemind4-4.9.2940/netbluemind/externaluser/api/
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-07-27 13:48:26.000000 netbluemind4-4.9.2940/netbluemind/externaluser/api/ExternalUser.py
+-rw-r--r--   0 root         (0) root         (0)     6976 2023-07-27 13:48:27.000000 netbluemind4-4.9.2940/netbluemind/externaluser/api/IExternalUser.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:12.000000 netbluemind4-4.9.2940/netbluemind/externaluser/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.605645 netbluemind4-4.9.2940/netbluemind/filehosting/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/filehosting/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.609645 netbluemind4-4.9.2940/netbluemind/filehosting/api/
+-rw-r--r--   0 root         (0) root         (0)     1835 2023-07-27 13:48:07.000000 netbluemind4-4.9.2940/netbluemind/filehosting/api/Configuration.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2023-07-27 13:48:07.000000 netbluemind4-4.9.2940/netbluemind/filehosting/api/FileHostingInfo.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-07-27 13:48:07.000000 netbluemind4-4.9.2940/netbluemind/filehosting/api/FileHostingInfoType.py
+-rw-r--r--   0 root         (0) root         (0)     3011 2023-07-27 13:48:07.000000 netbluemind4-4.9.2940/netbluemind/filehosting/api/FileHostingItem.py
+-rw-r--r--   0 root         (0) root         (0)     1802 2023-07-27 13:48:07.000000 netbluemind4-4.9.2940/netbluemind/filehosting/api/FileHostingPublicLink.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-07-27 13:48:07.000000 netbluemind4-4.9.2940/netbluemind/filehosting/api/FileType.py
+-rw-r--r--   0 root         (0) root         (0)     8093 2023-07-27 13:48:08.000000 netbluemind4-4.9.2940/netbluemind/filehosting/api/IFileHosting.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-07-27 13:48:07.000000 netbluemind4-4.9.2940/netbluemind/filehosting/api/IInternalBMFileSystem.py
+-rw-r--r--   0 root         (0) root         (0)     1686 2023-07-27 13:48:07.000000 netbluemind4-4.9.2940/netbluemind/filehosting/api/Metadata.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/filehosting/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.609645 netbluemind4-4.9.2940/netbluemind/group/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/group/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.609645 netbluemind4-4.9.2940/netbluemind/group/api/
+-rw-r--r--   0 root         (0) root         (0)     3205 2023-07-27 13:48:18.000000 netbluemind4-4.9.2940/netbluemind/group/api/Group.py
+-rw-r--r--   0 root         (0) root         (0)     1826 2023-07-27 13:48:18.000000 netbluemind4-4.9.2940/netbluemind/group/api/GroupSearchQuery.py
+-rw-r--r--   0 root         (0) root         (0)    16842 2023-07-27 13:48:18.000000 netbluemind4-4.9.2940/netbluemind/group/api/IGroup.py
+-rw-r--r--   0 root         (0) root         (0)     2253 2023-07-27 13:48:17.000000 netbluemind4-4.9.2940/netbluemind/group/api/IGroupMember.py
+-rw-r--r--   0 root         (0) root         (0)     1965 2023-07-27 13:48:18.000000 netbluemind4-4.9.2940/netbluemind/group/api/Member.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-07-27 13:48:18.000000 netbluemind4-4.9.2940/netbluemind/group/api/MemberType.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/group/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.609645 netbluemind4-4.9.2940/netbluemind/hsm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/hsm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.613645 netbluemind4-4.9.2940/netbluemind/hsm/api/
+-rw-r--r--   0 root         (0) root         (0)     1968 2023-07-27 13:48:18.000000 netbluemind4-4.9.2940/netbluemind/hsm/api/Demote.py
+-rw-r--r--   0 root         (0) root         (0)     3771 2023-07-27 13:48:19.000000 netbluemind4-4.9.2940/netbluemind/hsm/api/IHSM.py
+-rw-r--r--   0 root         (0) root         (0)     2714 2023-07-27 13:48:19.000000 netbluemind4-4.9.2940/netbluemind/hsm/api/Promote.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2023-07-27 13:48:18.000000 netbluemind4-4.9.2940/netbluemind/hsm/api/TierChangeResult.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/hsm/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.613645 netbluemind4-4.9.2940/netbluemind/icalendar/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/icalendar/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.613645 netbluemind4-4.9.2940/netbluemind/icalendar/api/
+-rw-r--r--   0 root         (0) root         (0)    11482 2023-07-27 13:48:34.000000 netbluemind4-4.9.2940/netbluemind/icalendar/api/ICalendarElement.py
+-rw-r--r--   0 root         (0) root         (0)     6703 2023-07-27 13:48:34.000000 netbluemind4-4.9.2940/netbluemind/icalendar/api/ICalendarElementAttendee.py
+-rw-r--r--   0 root         (0) root         (0)     1205 2023-07-27 13:48:34.000000 netbluemind4-4.9.2940/netbluemind/icalendar/api/ICalendarElementCUType.py
+-rw-r--r--   0 root         (0) root         (0)     1191 2023-07-27 13:48:34.000000 netbluemind4-4.9.2940/netbluemind/icalendar/api/ICalendarElementClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2199 2023-07-27 13:48:34.000000 netbluemind4-4.9.2940/netbluemind/icalendar/api/ICalendarElementOrganizer.py
+-rw-r--r--   0 root         (0) root         (0)     1294 2023-07-27 13:48:34.000000 netbluemind4-4.9.2940/netbluemind/icalendar/api/ICalendarElementParticipationStatus.py
+-rw-r--r--   0 root         (0) root         (0)     6113 2023-07-27 13:48:34.000000 netbluemind4-4.9.2940/netbluemind/icalendar/api/ICalendarElementRRule.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-07-27 13:48:34.000000 netbluemind4-4.9.2940/netbluemind/icalendar/api/ICalendarElementRRuleFrequency.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2023-07-27 13:48:34.000000 netbluemind4-4.9.2940/netbluemind/icalendar/api/ICalendarElementRRuleWeekDay.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-07-27 13:48:34.000000 netbluemind4-4.9.2940/netbluemind/icalendar/api/ICalendarElementRole.py
+-rw-r--r--   0 root         (0) root         (0)     1259 2023-07-27 13:48:34.000000 netbluemind4-4.9.2940/netbluemind/icalendar/api/ICalendarElementStatus.py
+-rw-r--r--   0 root         (0) root         (0)     3218 2023-07-27 13:48:34.000000 netbluemind4-4.9.2940/netbluemind/icalendar/api/ICalendarElementVAlarm.py
+-rw-r--r--   0 root         (0) root         (0)     1169 2023-07-27 13:48:34.000000 netbluemind4-4.9.2940/netbluemind/icalendar/api/ICalendarElementVAlarmAction.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/icalendar/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.613645 netbluemind4-4.9.2940/netbluemind/im/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/im/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.617646 netbluemind4-4.9.2940/netbluemind/im/api/
+-rw-r--r--   0 root         (0) root         (0)     3937 2023-07-27 13:47:53.000000 netbluemind4-4.9.2940/netbluemind/im/api/IInstantMessaging.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2023-07-27 13:47:53.000000 netbluemind4-4.9.2940/netbluemind/im/api/IMMessage.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/im/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.617646 netbluemind4-4.9.2940/netbluemind/mailbox/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/mailbox/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.621646 netbluemind4-4.9.2940/netbluemind/mailbox/api/
+-rw-r--r--   0 root         (0) root         (0)     1444 2023-07-27 13:48:23.000000 netbluemind4-4.9.2940/netbluemind/mailbox/api/IMailboxAclUids.py
+-rw-r--r--   0 root         (0) root         (0)     5008 2023-07-27 13:48:24.000000 netbluemind4-4.9.2940/netbluemind/mailbox/api/IMailboxMgmt.py
+-rw-r--r--   0 root         (0) root         (0)    17092 2023-07-27 13:48:25.000000 netbluemind4-4.9.2940/netbluemind/mailbox/api/IMailboxes.py
+-rw-r--r--   0 root         (0) root         (0)     3211 2023-07-27 13:48:25.000000 netbluemind4-4.9.2940/netbluemind/mailbox/api/MailFilter.py
+-rw-r--r--   0 root         (0) root         (0)     2069 2023-07-27 13:48:24.000000 netbluemind4-4.9.2940/netbluemind/mailbox/api/MailFilterForwarding.py
+-rw-r--r--   0 root         (0) root         (0)     3916 2023-07-27 13:48:23.000000 netbluemind4-4.9.2940/netbluemind/mailbox/api/MailFilterRule.py
+-rw-r--r--   0 root         (0) root         (0)     2616 2023-07-27 13:48:23.000000 netbluemind4-4.9.2940/netbluemind/mailbox/api/MailFilterVacation.py
+-rw-r--r--   0 root         (0) root         (0)     4279 2023-07-27 13:48:23.000000 netbluemind4-4.9.2940/netbluemind/mailbox/api/Mailbox.py
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-07-27 13:48:25.000000 netbluemind4-4.9.2940/netbluemind/mailbox/api/MailboxConfig.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2023-07-27 13:48:24.000000 netbluemind4-4.9.2940/netbluemind/mailbox/api/MailboxQuota.py
+-rw-r--r--   0 root         (0) root         (0)     1133 2023-07-27 13:48:24.000000 netbluemind4-4.9.2940/netbluemind/mailbox/api/MailboxRouting.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-07-27 13:48:24.000000 netbluemind4-4.9.2940/netbluemind/mailbox/api/MailboxType.py
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-07-27 13:48:23.000000 netbluemind4-4.9.2940/netbluemind/mailbox/api/ShardStats.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2023-07-27 13:48:23.000000 netbluemind4-4.9.2940/netbluemind/mailbox/api/ShardStatsMailboxStats.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-07-27 13:48:25.000000 netbluemind4-4.9.2940/netbluemind/mailbox/api/ShardStatsState.py
+-rw-r--r--   0 root         (0) root         (0)     3337 2023-07-27 13:48:25.000000 netbluemind4-4.9.2940/netbluemind/mailbox/api/SimpleShardStats.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/mailbox/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.621646 netbluemind4-4.9.2940/netbluemind/mailbox/identity/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/mailbox/identity/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.621646 netbluemind4-4.9.2940/netbluemind/mailbox/identity/api/
+-rw-r--r--   0 root         (0) root         (0)     5175 2023-07-27 13:48:25.000000 netbluemind4-4.9.2940/netbluemind/mailbox/identity/api/IMailboxIdentity.py
+-rw-r--r--   0 root         (0) root         (0)     3330 2023-07-27 13:48:25.000000 netbluemind4-4.9.2940/netbluemind/mailbox/identity/api/Identity.py
+-rw-r--r--   0 root         (0) root         (0)     3125 2023-07-27 13:48:25.000000 netbluemind4-4.9.2940/netbluemind/mailbox/identity/api/IdentityDescription.py
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-27 13:48:25.000000 netbluemind4-4.9.2940/netbluemind/mailbox/identity/api/SignatureFormat.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/mailbox/identity/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.621646 netbluemind4-4.9.2940/netbluemind/mailflow/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/mailflow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.621646 netbluemind4-4.9.2940/netbluemind/mailflow/common/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/mailflow/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.625646 netbluemind4-4.9.2940/netbluemind/mailflow/common/api/
+-rw-r--r--   0 root         (0) root         (0)     2218 2023-07-27 13:48:15.000000 netbluemind4-4.9.2940/netbluemind/mailflow/common/api/AssignmentActionMapping.py
+-rw-r--r--   0 root         (0) root         (0)     2849 2023-07-27 13:48:15.000000 netbluemind4-4.9.2940/netbluemind/mailflow/common/api/Message.py
+-rw-r--r--   0 root         (0) root         (0)     3164 2023-07-27 13:48:15.000000 netbluemind4-4.9.2940/netbluemind/mailflow/common/api/Recipient.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-07-27 13:48:15.000000 netbluemind4-4.9.2940/netbluemind/mailflow/common/api/RecipientAddressType.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-07-27 13:48:15.000000 netbluemind4-4.9.2940/netbluemind/mailflow/common/api/RecipientRecipientType.py
+-rw-r--r--   0 root         (0) root         (0)     1714 2023-07-27 13:48:15.000000 netbluemind4-4.9.2940/netbluemind/mailflow/common/api/SendingAs.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:10.000000 netbluemind4-4.9.2940/netbluemind/mailflow/common/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.625646 netbluemind4-4.9.2940/netbluemind/mailmessage/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:12.000000 netbluemind4-4.9.2940/netbluemind/mailmessage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.625646 netbluemind4-4.9.2940/netbluemind/mailmessage/api/
+-rw-r--r--   0 root         (0) root         (0)     1928 2023-07-27 13:48:35.000000 netbluemind4-4.9.2940/netbluemind/mailmessage/api/IMailTip.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2023-07-27 13:48:35.000000 netbluemind4-4.9.2940/netbluemind/mailmessage/api/MailTip.py
+-rw-r--r--   0 root         (0) root         (0)     2531 2023-07-27 13:48:35.000000 netbluemind4-4.9.2940/netbluemind/mailmessage/api/MailTipContext.py
+-rw-r--r--   0 root         (0) root         (0)     2316 2023-07-27 13:48:35.000000 netbluemind4-4.9.2940/netbluemind/mailmessage/api/MailTipFilter.py
+-rw-r--r--   0 root         (0) root         (0)     1138 2023-07-27 13:48:35.000000 netbluemind4-4.9.2940/netbluemind/mailmessage/api/MailTipFilterFilterType.py
+-rw-r--r--   0 root         (0) root         (0)     2519 2023-07-27 13:48:35.000000 netbluemind4-4.9.2940/netbluemind/mailmessage/api/MailTips.py
+-rw-r--r--   0 root         (0) root         (0)     3062 2023-07-27 13:48:35.000000 netbluemind4-4.9.2940/netbluemind/mailmessage/api/MessageContext.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:12.000000 netbluemind4-4.9.2940/netbluemind/mailmessage/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.625646 netbluemind4-4.9.2940/netbluemind/mailshare/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:12.000000 netbluemind4-4.9.2940/netbluemind/mailshare/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.629646 netbluemind4-4.9.2940/netbluemind/mailshare/api/
+-rw-r--r--   0 root         (0) root         (0)     6859 2023-07-27 13:48:17.000000 netbluemind4-4.9.2940/netbluemind/mailshare/api/IMailshare.py
+-rw-r--r--   0 root         (0) root         (0)     3056 2023-07-27 13:48:16.000000 netbluemind4-4.9.2940/netbluemind/mailshare/api/Mailshare.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:12.000000 netbluemind4-4.9.2940/netbluemind/mailshare/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.629646 netbluemind4-4.9.2940/netbluemind/notes/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:14.000000 netbluemind4-4.9.2940/netbluemind/notes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.629646 netbluemind4-4.9.2940/netbluemind/notes/api/
+-rw-r--r--   0 root         (0) root         (0)    19475 2023-07-27 13:48:07.000000 netbluemind4-4.9.2940/netbluemind/notes/api/INote.py
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-07-27 13:48:05.000000 netbluemind4-4.9.2940/netbluemind/notes/api/INoteIndexMgmt.py
+-rw-r--r--   0 root         (0) root         (0)     1942 2023-07-27 13:48:07.000000 netbluemind4-4.9.2940/netbluemind/notes/api/INoteUids.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2023-07-27 13:48:05.000000 netbluemind4-4.9.2940/netbluemind/notes/api/INotes.py
+-rw-r--r--   0 root         (0) root         (0)     3598 2023-07-27 13:48:07.000000 netbluemind4-4.9.2940/netbluemind/notes/api/VNote.py
+-rw-r--r--   0 root         (0) root         (0)     3333 2023-07-27 13:48:07.000000 netbluemind4-4.9.2940/netbluemind/notes/api/VNoteChanges.py
+-rw-r--r--   0 root         (0) root         (0)     2290 2023-07-27 13:48:05.000000 netbluemind4-4.9.2940/netbluemind/notes/api/VNoteChangesItemAdd.py
+-rw-r--r--   0 root         (0) root         (0)     1842 2023-07-27 13:48:07.000000 netbluemind4-4.9.2940/netbluemind/notes/api/VNoteChangesItemDelete.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-07-27 13:48:07.000000 netbluemind4-4.9.2940/netbluemind/notes/api/VNoteChangesItemModify.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2023-07-27 13:48:07.000000 netbluemind4-4.9.2940/netbluemind/notes/api/VNoteColor.py
+-rw-r--r--   0 root         (0) root         (0)     2169 2023-07-27 13:48:07.000000 netbluemind4-4.9.2940/netbluemind/notes/api/VNoteQuery.py
+-rw-r--r--   0 root         (0) root         (0)     2374 2023-07-27 13:48:07.000000 netbluemind4-4.9.2940/netbluemind/notes/api/VNotesQuery.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:14.000000 netbluemind4-4.9.2940/netbluemind/notes/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.629646 netbluemind4-4.9.2940/netbluemind/python/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-01-23 11:00:08.000000 netbluemind4-4.9.2940/netbluemind/python/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4632 2023-07-27 13:48:17.000000 netbluemind4-4.9.2940/netbluemind/python/client.py
+-rw-r--r--   0 root         (0) root         (0)     4129 2023-07-27 13:48:17.000000 netbluemind4-4.9.2940/netbluemind/python/serder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.629646 netbluemind4-4.9.2940/netbluemind/resource/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:12.000000 netbluemind4-4.9.2940/netbluemind/resource/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.633646 netbluemind4-4.9.2940/netbluemind/resource/api/
+-rw-r--r--   0 root         (0) root         (0)     1281 2023-07-27 13:48:19.000000 netbluemind4-4.9.2940/netbluemind/resource/api/EventInfo.py
+-rw-r--r--   0 root         (0) root         (0)     7985 2023-07-27 13:48:19.000000 netbluemind4-4.9.2940/netbluemind/resource/api/IResources.py
+-rw-r--r--   0 root         (0) root         (0)     3991 2023-07-27 13:48:19.000000 netbluemind4-4.9.2940/netbluemind/resource/api/ResourceDescriptor.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-07-27 13:48:19.000000 netbluemind4-4.9.2940/netbluemind/resource/api/ResourceDescriptorPropertyValue.py
+-rw-r--r--   0 root         (0) root         (0)     1204 2023-07-27 13:48:19.000000 netbluemind4-4.9.2940/netbluemind/resource/api/ResourceReservationMode.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:12.000000 netbluemind4-4.9.2940/netbluemind/resource/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.633646 netbluemind4-4.9.2940/netbluemind/resource/api/type/
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-07-27 13:48:19.000000 netbluemind4-4.9.2940/netbluemind/resource/api/type/IResourceTypeUids.py
+-rw-r--r--   0 root         (0) root         (0)     5685 2023-07-27 13:48:20.000000 netbluemind4-4.9.2940/netbluemind/resource/api/type/IResourceTypes.py
+-rw-r--r--   0 root         (0) root         (0)     1761 2023-07-27 13:48:19.000000 netbluemind4-4.9.2940/netbluemind/resource/api/type/ResourceType.py
+-rw-r--r--   0 root         (0) root         (0)     2692 2023-07-27 13:48:19.000000 netbluemind4-4.9.2940/netbluemind/resource/api/type/ResourceTypeDescriptor.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-07-27 13:48:19.000000 netbluemind4-4.9.2940/netbluemind/resource/api/type/ResourceTypeDescriptorProperty.py
+-rw-r--r--   0 root         (0) root         (0)     1191 2023-07-27 13:48:19.000000 netbluemind4-4.9.2940/netbluemind/resource/api/type/ResourceTypeDescriptorPropertyType.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:12.000000 netbluemind4-4.9.2940/netbluemind/resource/api/type/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.633646 netbluemind4-4.9.2940/netbluemind/role/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:12.000000 netbluemind4-4.9.2940/netbluemind/role/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.633646 netbluemind4-4.9.2940/netbluemind/role/api/
+-rw-r--r--   0 root         (0) root         (0)     2151 2023-07-27 13:48:26.000000 netbluemind4-4.9.2940/netbluemind/role/api/IRoles.py
+-rw-r--r--   0 root         (0) root         (0)     5403 2023-07-27 13:48:26.000000 netbluemind4-4.9.2940/netbluemind/role/api/RoleDescriptor.py
+-rw-r--r--   0 root         (0) root         (0)     1926 2023-07-27 13:48:26.000000 netbluemind4-4.9.2940/netbluemind/role/api/RolesCategory.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:12.000000 netbluemind4-4.9.2940/netbluemind/role/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.633646 netbluemind4-4.9.2940/netbluemind/scheduledjob/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:12.000000 netbluemind4-4.9.2940/netbluemind/scheduledjob/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.637646 netbluemind4-4.9.2940/netbluemind/scheduledjob/api/
+-rw-r--r--   0 root         (0) root         (0)     7252 2023-07-27 13:48:34.000000 netbluemind4-4.9.2940/netbluemind/scheduledjob/api/IJob.py
+-rw-r--r--   0 root         (0) root         (0)     4227 2023-07-27 13:48:34.000000 netbluemind4-4.9.2940/netbluemind/scheduledjob/api/Job.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2023-07-27 13:48:33.000000 netbluemind4-4.9.2940/netbluemind/scheduledjob/api/JobDomainStatus.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2023-07-27 13:48:34.000000 netbluemind4-4.9.2940/netbluemind/scheduledjob/api/JobExecution.py
+-rw-r--r--   0 root         (0) root         (0)     3201 2023-07-27 13:48:34.000000 netbluemind4-4.9.2940/netbluemind/scheduledjob/api/JobExecutionQuery.py
+-rw-r--r--   0 root         (0) root         (0)     1252 2023-07-27 13:48:33.000000 netbluemind4-4.9.2940/netbluemind/scheduledjob/api/JobExitStatus.py
+-rw-r--r--   0 root         (0) root         (0)     1096 2023-07-27 13:48:34.000000 netbluemind4-4.9.2940/netbluemind/scheduledjob/api/JobKind.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-07-27 13:48:34.000000 netbluemind4-4.9.2940/netbluemind/scheduledjob/api/JobPlanification.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-07-27 13:48:33.000000 netbluemind4-4.9.2940/netbluemind/scheduledjob/api/JobQuery.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-07-27 13:48:33.000000 netbluemind4-4.9.2940/netbluemind/scheduledjob/api/JobRec.py
+-rw-r--r--   0 root         (0) root         (0)     2734 2023-07-27 13:48:34.000000 netbluemind4-4.9.2940/netbluemind/scheduledjob/api/LogEntry.py
+-rw-r--r--   0 root         (0) root         (0)     1133 2023-07-27 13:48:33.000000 netbluemind4-4.9.2940/netbluemind/scheduledjob/api/LogLevel.py
+-rw-r--r--   0 root         (0) root         (0)     1135 2023-07-27 13:48:34.000000 netbluemind4-4.9.2940/netbluemind/scheduledjob/api/PlanKind.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:12.000000 netbluemind4-4.9.2940/netbluemind/scheduledjob/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.637646 netbluemind4-4.9.2940/netbluemind/server/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:12.000000 netbluemind4-4.9.2940/netbluemind/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.641646 netbluemind4-4.9.2940/netbluemind/server/api/
+-rw-r--r--   0 root         (0) root         (0)     1977 2023-07-27 13:48:25.000000 netbluemind4-4.9.2940/netbluemind/server/api/Assignment.py
+-rw-r--r--   0 root         (0) root         (0)     2093 2023-07-27 13:48:26.000000 netbluemind4-4.9.2940/netbluemind/server/api/CommandStatus.py
+-rw-r--r--   0 root         (0) root         (0)    12017 2023-07-27 13:48:26.000000 netbluemind4-4.9.2940/netbluemind/server/api/IServer.py
+-rw-r--r--   0 root         (0) root         (0)     2108 2023-07-27 13:48:26.000000 netbluemind4-4.9.2940/netbluemind/server/api/Server.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:12.000000 netbluemind4-4.9.2940/netbluemind/server/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.641646 netbluemind4-4.9.2940/netbluemind/system/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:12.000000 netbluemind4-4.9.2940/netbluemind/system/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.649646 netbluemind4-4.9.2940/netbluemind/system/api/
+-rw-r--r--   0 root         (0) root         (0)     3513 2023-07-27 13:48:38.000000 netbluemind4-4.9.2940/netbluemind/system/api/CertData.py
+-rw-r--r--   0 root         (0) root         (0)     1192 2023-07-27 13:48:37.000000 netbluemind4-4.9.2940/netbluemind/system/api/CertDataCertificateDomainEngine.py
+-rw-r--r--   0 root         (0) root         (0)     4088 2023-07-27 13:48:39.000000 netbluemind4-4.9.2940/netbluemind/system/api/CloneConfiguration.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2023-07-27 13:48:39.000000 netbluemind4-4.9.2940/netbluemind/system/api/CloneConfigurationMode.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2023-07-27 13:48:38.000000 netbluemind4-4.9.2940/netbluemind/system/api/ConnectionTestStatus.py
+-rw-r--r--   0 root         (0) root         (0)     1764 2023-07-27 13:48:36.000000 netbluemind4-4.9.2940/netbluemind/system/api/CustomLogo.py
+-rw-r--r--   0 root         (0) root         (0)     1951 2023-07-27 13:48:36.000000 netbluemind4-4.9.2940/netbluemind/system/api/DomainTemplate.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2023-07-27 13:48:38.000000 netbluemind4-4.9.2940/netbluemind/system/api/DomainTemplateDescription.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-07-27 13:48:38.000000 netbluemind4-4.9.2940/netbluemind/system/api/DomainTemplateDescriptionI18NDescription.py
+-rw-r--r--   0 root         (0) root         (0)     2858 2023-07-27 13:48:38.000000 netbluemind4-4.9.2940/netbluemind/system/api/DomainTemplateKind.py
+-rw-r--r--   0 root         (0) root         (0)     2999 2023-07-27 13:48:36.000000 netbluemind4-4.9.2940/netbluemind/system/api/DomainTemplateTag.py
+-rw-r--r--   0 root         (0) root         (0)     2812 2023-07-27 13:48:39.000000 netbluemind4-4.9.2940/netbluemind/system/api/ExternalSystem.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2023-07-27 13:48:38.000000 netbluemind4-4.9.2940/netbluemind/system/api/ExternalSystemAuthKind.py
+-rw-r--r--   0 root         (0) root         (0)     1764 2023-07-27 13:48:39.000000 netbluemind4-4.9.2940/netbluemind/system/api/ICacheMgmt.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-07-27 13:48:38.000000 netbluemind4-4.9.2940/netbluemind/system/api/ICustomTheme.py
+-rw-r--r--   0 root         (0) root         (0)     1545 2023-07-27 13:48:38.000000 netbluemind4-4.9.2940/netbluemind/system/api/IDomainTemplate.py
+-rw-r--r--   0 root         (0) root         (0)     4877 2023-07-27 13:48:37.000000 netbluemind4-4.9.2940/netbluemind/system/api/IExternalSystem.py
+-rw-r--r--   0 root         (0) root         (0)     2369 2023-07-27 13:48:39.000000 netbluemind4-4.9.2940/netbluemind/system/api/IGlobalSettings.py
+-rw-r--r--   0 root         (0) root         (0)    17153 2023-07-27 13:48:38.000000 netbluemind4-4.9.2940/netbluemind/system/api/IInstallation.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-07-27 13:48:37.000000 netbluemind4-4.9.2940/netbluemind/system/api/IMailDeliveryMgmt.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-07-27 13:48:37.000000 netbluemind4-4.9.2940/netbluemind/system/api/ISchemaMgmt.py
+-rw-r--r--   0 root         (0) root         (0)     4029 2023-07-27 13:48:38.000000 netbluemind4-4.9.2940/netbluemind/system/api/ISecurityMgmt.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-07-27 13:48:39.000000 netbluemind4-4.9.2940/netbluemind/system/api/ISystemConfiguration.py
+-rw-r--r--   0 root         (0) root         (0)     2488 2023-07-27 13:48:36.000000 netbluemind4-4.9.2940/netbluemind/system/api/InstallationVersion.py
+-rw-r--r--   0 root         (0) root         (0)     2155 2023-07-27 13:48:37.000000 netbluemind4-4.9.2940/netbluemind/system/api/PublicInfos.py
+-rw-r--r--   0 root         (0) root         (0)     1965 2023-07-27 13:48:39.000000 netbluemind4-4.9.2940/netbluemind/system/api/SchemaCheckInfo.py
+-rw-r--r--   0 root         (0) root         (0)     7282 2023-07-27 13:48:36.000000 netbluemind4-4.9.2940/netbluemind/system/api/SubscriptionInformations.py
+-rw-r--r--   0 root         (0) root         (0)     3048 2023-07-27 13:48:37.000000 netbluemind4-4.9.2940/netbluemind/system/api/SubscriptionInformationsInstallationIndicator.py
+-rw-r--r--   0 root         (0) root         (0)     1266 2023-07-27 13:48:39.000000 netbluemind4-4.9.2940/netbluemind/system/api/SubscriptionInformationsInstallationIndicatorKind.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-07-27 13:48:39.000000 netbluemind4-4.9.2940/netbluemind/system/api/SubscriptionInformationsKind.py
+-rw-r--r--   0 root         (0) root         (0)     3108 2023-07-27 13:48:39.000000 netbluemind4-4.9.2940/netbluemind/system/api/SubscriptionInformationsMessage.py
+-rw-r--r--   0 root         (0) root         (0)     1248 2023-07-27 13:48:38.000000 netbluemind4-4.9.2940/netbluemind/system/api/SubscriptionInformationsMessageCode.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-07-27 13:48:39.000000 netbluemind4-4.9.2940/netbluemind/system/api/SubscriptionInformationsMessageKind.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-07-27 13:48:38.000000 netbluemind4-4.9.2940/netbluemind/system/api/SystemConf.py
+-rw-r--r--   0 root         (0) root         (0)     1492 2023-07-27 13:48:36.000000 netbluemind4-4.9.2940/netbluemind/system/api/SystemState.py
+-rw-r--r--   0 root         (0) root         (0)     2684 2023-07-27 13:48:38.000000 netbluemind4-4.9.2940/netbluemind/system/api/UpgradeReport.py
+-rw-r--r--   0 root         (0) root         (0)     1114 2023-07-27 13:48:38.000000 netbluemind4-4.9.2940/netbluemind/system/api/UpgradeReportStatus.py
+-rw-r--r--   0 root         (0) root         (0)     1945 2023-07-27 13:48:39.000000 netbluemind4-4.9.2940/netbluemind/system/api/UpgradeReportUpgraderReport.py
+-rw-r--r--   0 root         (0) root         (0)     2115 2023-07-27 13:48:36.000000 netbluemind4-4.9.2940/netbluemind/system/api/UpgradeStatus.py
+-rw-r--r--   0 root         (0) root         (0)     1199 2023-07-27 13:48:38.000000 netbluemind4-4.9.2940/netbluemind/system/api/UpgradeStatusState.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:12.000000 netbluemind4-4.9.2940/netbluemind/system/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.649646 netbluemind4-4.9.2940/netbluemind/system/api/hot/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:12.000000 netbluemind4-4.9.2940/netbluemind/system/api/hot/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.653646 netbluemind4-4.9.2940/netbluemind/system/api/hot/upgrade/
+-rw-r--r--   0 root         (0) root         (0)     2466 2023-07-27 13:48:40.000000 netbluemind4-4.9.2940/netbluemind/system/api/hot/upgrade/HotUpgradeProgress.py
+-rw-r--r--   0 root         (0) root         (0)     5047 2023-07-27 13:48:39.000000 netbluemind4-4.9.2940/netbluemind/system/api/hot/upgrade/HotUpgradeTask.py
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-07-27 13:48:40.000000 netbluemind4-4.9.2940/netbluemind/system/api/hot/upgrade/HotUpgradeTaskExecutionMode.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-07-27 13:48:39.000000 netbluemind4-4.9.2940/netbluemind/system/api/hot/upgrade/HotUpgradeTaskFilter.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-07-27 13:48:39.000000 netbluemind4-4.9.2940/netbluemind/system/api/hot/upgrade/HotUpgradeTaskStatus.py
+-rw-r--r--   0 root         (0) root         (0)     3211 2023-07-27 13:48:40.000000 netbluemind4-4.9.2940/netbluemind/system/api/hot/upgrade/IHotUpgrade.py
+-rw-r--r--   0 root         (0) root         (0)     5213 2023-07-27 13:48:39.000000 netbluemind4-4.9.2940/netbluemind/system/api/hot/upgrade/IInternalHotUpgrade.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:12.000000 netbluemind4-4.9.2940/netbluemind/system/api/hot/upgrade/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.653646 netbluemind4-4.9.2940/netbluemind/tag/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:12.000000 netbluemind4-4.9.2940/netbluemind/tag/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.653646 netbluemind4-4.9.2940/netbluemind/tag/api/
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-07-27 13:48:20.000000 netbluemind4-4.9.2940/netbluemind/tag/api/ITagUids.py
+-rw-r--r--   0 root         (0) root         (0)     7936 2023-07-27 13:48:20.000000 netbluemind4-4.9.2940/netbluemind/tag/api/ITags.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-07-27 13:48:20.000000 netbluemind4-4.9.2940/netbluemind/tag/api/Tag.py
+-rw-r--r--   0 root         (0) root         (0)     3243 2023-07-27 13:48:20.000000 netbluemind4-4.9.2940/netbluemind/tag/api/TagChanges.py
+-rw-r--r--   0 root         (0) root         (0)     1929 2023-07-27 13:48:20.000000 netbluemind4-4.9.2940/netbluemind/tag/api/TagChangesItemAdd.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2023-07-27 13:48:20.000000 netbluemind4-4.9.2940/netbluemind/tag/api/TagChangesItemDelete.py
+-rw-r--r--   0 root         (0) root         (0)     1938 2023-07-27 13:48:20.000000 netbluemind4-4.9.2940/netbluemind/tag/api/TagChangesItemModify.py
+-rw-r--r--   0 root         (0) root         (0)     2205 2023-07-27 13:48:20.000000 netbluemind4-4.9.2940/netbluemind/tag/api/TagRef.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:12.000000 netbluemind4-4.9.2940/netbluemind/tag/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.653646 netbluemind4-4.9.2940/netbluemind/todolist/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:12.000000 netbluemind4-4.9.2940/netbluemind/todolist/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.657647 netbluemind4-4.9.2940/netbluemind/todolist/api/
+-rw-r--r--   0 root         (0) root         (0)    21899 2023-07-27 13:48:22.000000 netbluemind4-4.9.2940/netbluemind/todolist/api/ITodoList.py
+-rw-r--r--   0 root         (0) root         (0)     3303 2023-07-27 13:48:21.000000 netbluemind4-4.9.2940/netbluemind/todolist/api/ITodoLists.py
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-07-27 13:48:23.000000 netbluemind4-4.9.2940/netbluemind/todolist/api/ITodoListsMgmt.py
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-07-27 13:48:22.000000 netbluemind4-4.9.2940/netbluemind/todolist/api/ITodoUids.py
+-rw-r--r--   0 root         (0) root         (0)     2634 2023-07-27 13:48:21.000000 netbluemind4-4.9.2940/netbluemind/todolist/api/IVTodo.py
+-rw-r--r--   0 root         (0) root         (0)     2410 2023-07-27 13:48:22.000000 netbluemind4-4.9.2940/netbluemind/todolist/api/TodoListsVTodoQuery.py
+-rw-r--r--   0 root         (0) root         (0)     3104 2023-07-27 13:48:21.000000 netbluemind4-4.9.2940/netbluemind/todolist/api/VTodo.py
+-rw-r--r--   0 root         (0) root         (0)     3369 2023-07-27 13:48:22.000000 netbluemind4-4.9.2940/netbluemind/todolist/api/VTodoChanges.py
+-rw-r--r--   0 root         (0) root         (0)     2302 2023-07-27 13:48:21.000000 netbluemind4-4.9.2940/netbluemind/todolist/api/VTodoChangesItemAdd.py
+-rw-r--r--   0 root         (0) root         (0)     1842 2023-07-27 13:48:21.000000 netbluemind4-4.9.2940/netbluemind/todolist/api/VTodoChangesItemDelete.py
+-rw-r--r--   0 root         (0) root         (0)     2538 2023-07-27 13:48:21.000000 netbluemind4-4.9.2940/netbluemind/todolist/api/VTodoChangesItemModify.py
+-rw-r--r--   0 root         (0) root         (0)     3482 2023-07-27 13:48:21.000000 netbluemind4-4.9.2940/netbluemind/todolist/api/VTodoQuery.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:12.000000 netbluemind4-4.9.2940/netbluemind/todolist/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.657647 netbluemind4-4.9.2940/netbluemind/user/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:12.000000 netbluemind4-4.9.2940/netbluemind/user/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.657647 netbluemind4-4.9.2940/netbluemind/user/api/
+-rw-r--r--   0 root         (0) root         (0)     1879 2023-07-27 13:48:27.000000 netbluemind4-4.9.2940/netbluemind/user/api/ChangePassword.py
+-rw-r--r--   0 root         (0) root         (0)    16565 2023-07-27 13:48:28.000000 netbluemind4-4.9.2940/netbluemind/user/api/IUser.py
+-rw-r--r--   0 root         (0) root         (0)     4869 2023-07-27 13:48:29.000000 netbluemind4-4.9.2940/netbluemind/user/api/IUserExternalAccount.py
+-rw-r--r--   0 root         (0) root         (0)     5750 2023-07-27 13:48:29.000000 netbluemind4-4.9.2940/netbluemind/user/api/IUserMailIdentities.py
+-rw-r--r--   0 root         (0) root         (0)     3402 2023-07-27 13:48:29.000000 netbluemind4-4.9.2940/netbluemind/user/api/IUserSettings.py
+-rw-r--r--   0 root         (0) root         (0)     3990 2023-07-27 13:48:28.000000 netbluemind4-4.9.2940/netbluemind/user/api/IUserSubscription.py
+-rw-r--r--   0 root         (0) root         (0)     5804 2023-07-27 13:48:27.000000 netbluemind4-4.9.2940/netbluemind/user/api/User.py
+-rw-r--r--   0 root         (0) root         (0)     2159 2023-07-27 13:48:29.000000 netbluemind4-4.9.2940/netbluemind/user/api/UserAccount.py
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-07-27 13:48:27.000000 netbluemind4-4.9.2940/netbluemind/user/api/UserAccountInfo.py
+-rw-r--r--   0 root         (0) root         (0)     1861 2023-07-27 13:48:29.000000 netbluemind4-4.9.2940/netbluemind/user/api/UserMailIdentity.py
+-rw-r--r--   0 root         (0) root         (0)     1561 2023-07-27 13:48:27.000000 netbluemind4-4.9.2940/netbluemind/user/api/UserSettings.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:12.000000 netbluemind4-4.9.2940/netbluemind/user/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.657647 netbluemind4-4.9.2940/netbluemind/webappdata/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:14.000000 netbluemind4-4.9.2940/netbluemind/webappdata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.661647 netbluemind4-4.9.2940/netbluemind/webappdata/api/
+-rw-r--r--   0 root         (0) root         (0)    13653 2023-07-27 13:48:16.000000 netbluemind4-4.9.2940/netbluemind/webappdata/api/IWebAppData.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-07-27 13:48:16.000000 netbluemind4-4.9.2940/netbluemind/webappdata/api/IWebAppDataUids.py
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-07-27 13:48:16.000000 netbluemind4-4.9.2940/netbluemind/webappdata/api/WebAppData.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 09:19:14.000000 netbluemind4-4.9.2940/netbluemind/webappdata/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:48:42.661647 netbluemind4-4.9.2940/netbluemind4.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      534 2023-07-27 13:48:42.000000 netbluemind4-4.9.2940/netbluemind4.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    24380 2023-07-27 13:48:42.000000 netbluemind4-4.9.2940/netbluemind4.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 13:48:42.000000 netbluemind4-4.9.2940/netbluemind4.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-27 13:48:42.000000 netbluemind4-4.9.2940/netbluemind4.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-27 13:48:42.000000 netbluemind4-4.9.2940/netbluemind4.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-07-27 13:48:42.661647 netbluemind4-4.9.2940/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      813 2023-07-27 13:48:42.000000 netbluemind4-4.9.2940/setup.py
```

### Comparing `netbluemind4-4.9.2928/LICENSE.txt` & `netbluemind4-4.9.2940/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/PKG-INFO` & `netbluemind4-4.9.2940/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbluemind4
-Version: 4.9.2928
+Version: 4.9.2940
 Summary: Automatically generated client for BlueMind >= 4 REST API. Check netbluemind for older releases
 Home-page: http://git.blue-mind.net/bluemind/
 Author: BlueMind team
 Author-email: contact@bluemind.net
 Keywords: bluemind,rest,api,mail,groupware
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/AddressBookDescriptor.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/AddressBookDescriptor.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/IAddressBook.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/IAddressBook.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IAddressBook_VERSION = "4.9.2928"
+IAddressBook_VERSION = "4.9.2940"
 
 
 class IAddressBook(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/addressbooks/{containerUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/IAddressBookUids.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/IAddressBookUids.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IAddressBookUids_VERSION = "4.9.2928"
+IAddressBookUids_VERSION = "4.9.2940"
 
 
 class IAddressBookUids(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/addressbook/uids'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/IAddressBooks.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/IAddressBooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IAddressBooks_VERSION = "4.9.2928"
+IAddressBooks_VERSION = "4.9.2940"
 
 
 class IAddressBooks(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/addressbooks'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/IAddressBooksMgmt.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/IAddressBooksMgmt.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IAddressBooksMgmt_VERSION = "4.9.2928"
+IAddressBooksMgmt_VERSION = "4.9.2940"
 
 
 class IAddressBooksMgmt(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mgmt/addressbooks'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/IVCardService.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/IVCardService.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IVCardService_VERSION = "4.9.2928"
+IVCardService_VERSION = "4.9.2940"
 
 
 class IVCardService(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/addressbooks/vcards/{containerUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCard.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCard.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardBasicAttribute.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardBasicAttribute.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardChanges.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardChanges.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardChangesItemAdd.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardChangesItemAdd.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardChangesItemDelete.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardChangesItemDelete.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardChangesItemModify.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardChangesItemModify.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardCommunications.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardCommunications.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardCommunicationsEmail.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardCommunicationsEmail.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardCommunicationsImpp.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardCommunicationsImpp.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardCommunicationsLang.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardCommunicationsLang.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardCommunicationsTel.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardCommunicationsTel.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardDeliveryAddressing.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardDeliveryAddressing.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardDeliveryAddressingAddress.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardDeliveryAddressingAddress.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardExplanatory.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardExplanatory.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardExplanatoryUrl.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardExplanatoryUrl.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardIdentification.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardIdentification.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardIdentificationFormatedName.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardIdentificationFormatedName.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardIdentificationGender.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardIdentificationGender.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardIdentificationName.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardIdentificationName.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardIdentificationNickname.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardIdentificationNickname.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardInfo.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardInfo.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardKind.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardKind.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardOrganizational.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardOrganizational.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardOrganizationalMember.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardOrganizationalMember.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardOrganizationalOrg.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardOrganizationalOrg.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardParameter.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardParameter.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardQuery.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardQueryOrderBy.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardQueryOrderBy.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardRelated.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardRelated.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardSecurity.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardSecurity.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/addressbook/api/VCardSecurityKey.py` & `netbluemind4-4.9.2940/netbluemind/addressbook/api/VCardSecurityKey.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/attachment/api/AttachedFile.py` & `netbluemind4-4.9.2940/netbluemind/attachment/api/AttachedFile.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/attachment/api/Configuration.py` & `netbluemind4-4.9.2940/netbluemind/attachment/api/Configuration.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/attachment/api/IAttachment.py` & `netbluemind4-4.9.2940/netbluemind/attachment/api/IAttachment.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IAttachment_VERSION = "4.9.2928"
+IAttachment_VERSION = "4.9.2940"
 
 
 class IAttachment(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/attachment/{domainUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/authentication/api/APIKey.py` & `netbluemind4-4.9.2940/netbluemind/authentication/api/APIKey.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/authentication/api/AccessTokenInfo.py` & `netbluemind4-4.9.2940/netbluemind/authentication/api/AccessTokenInfo.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/authentication/api/AccessTokenInfoTokenStatus.py` & `netbluemind4-4.9.2940/netbluemind/authentication/api/AccessTokenInfoTokenStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/authentication/api/AuthUser.py` & `netbluemind4-4.9.2940/netbluemind/authentication/api/AuthUser.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/authentication/api/IAPIKeys.py` & `netbluemind4-4.9.2940/netbluemind/authentication/api/IAPIKeys.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IAPIKeys_VERSION = "4.9.2928"
+IAPIKeys_VERSION = "4.9.2940"
 
 
 class IAPIKeys(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/auth/keys'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/authentication/api/IAuthentication.py` & `netbluemind4-4.9.2940/netbluemind/authentication/api/IAuthentication.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IAuthentication_VERSION = "4.9.2928"
+IAuthentication_VERSION = "4.9.2940"
 
 
 class IAuthentication(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/auth'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/authentication/api/ISecurityToken.py` & `netbluemind4-4.9.2940/netbluemind/authentication/api/ISecurityToken.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ISecurityToken_VERSION = "4.9.2928"
+ISecurityToken_VERSION = "4.9.2940"
 
 
 class ISecurityToken(BaseEndpoint):
     def __init__(self, apiKey, url, sessionIdentifier):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/auth/token/{sessionIdentifier}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/authentication/api/ISudoSupport.py` & `netbluemind4-4.9.2940/netbluemind/authentication/api/ISudoSupport.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ISudoSupport_VERSION = "4.9.2928"
+ISudoSupport_VERSION = "4.9.2940"
 
 
 class ISudoSupport(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/auth/sudo_support'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/authentication/api/IUserAccessToken.py` & `netbluemind4-4.9.2940/netbluemind/authentication/api/IUserAccessToken.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IUserAccessToken_VERSION = "4.9.2928"
+IUserAccessToken_VERSION = "4.9.2940"
 
 
 class IUserAccessToken(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/auth/access_token'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/authentication/api/LoginResponse.py` & `netbluemind4-4.9.2940/netbluemind/authentication/api/LoginResponse.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/authentication/api/LoginResponseStatus.py` & `netbluemind4-4.9.2940/netbluemind/authentication/api/LoginResponseStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/authentication/api/ValidationKind.py` & `netbluemind4-4.9.2940/netbluemind/authentication/api/ValidationKind.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/Conversation.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/Conversation.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/ConversationMessageRef.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/ConversationMessageRef.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/DispositionType.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/DispositionType.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/IBaseMailboxFolders.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/IBaseMailboxFolders.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IBaseMailboxFolders_VERSION = "4.9.2928"
+IBaseMailboxFolders_VERSION = "4.9.2940"
 
 
 class IBaseMailboxFolders(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + ''
```

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/IItemsTransfer.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/IItemsTransfer.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IItemsTransfer_VERSION = "4.9.2928"
+IItemsTransfer_VERSION = "4.9.2940"
 
 
 class IItemsTransfer(BaseEndpoint):
     def __init__(self, apiKey, url, fromMailboxUid, toMailboxUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + \
```

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/IMailConversation.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/IMailConversation.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IMailConversation_VERSION = "4.9.2928"
+IMailConversation_VERSION = "4.9.2940"
 
 
 class IMailConversation(BaseEndpoint):
     def __init__(self, apiKey, url, conversationContainer):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mail_conversation/{conversationContainer}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/IMailConversationActions.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/IMailConversationActions.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IMailConversationActions_VERSION = "4.9.2928"
+IMailConversationActions_VERSION = "4.9.2940"
 
 
 class IMailConversationActions(BaseEndpoint):
     def __init__(self, apiKey, url, conversationContainer, replicatedMailboxUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + \
```

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/IMailboxFolders.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/IMailboxFolders.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IMailboxFolders_VERSION = "4.9.2928"
+IMailboxFolders_VERSION = "4.9.2940"
 
 
 class IMailboxFolders(BaseEndpoint):
     def __init__(self, apiKey, url, partition, mailboxRoot):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mail_folders/{partition}/{mailboxRoot}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/IMailboxFoldersByContainer.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/IMailboxFoldersByContainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IMailboxFoldersByContainer_VERSION = "4.9.2928"
+IMailboxFoldersByContainer_VERSION = "4.9.2940"
 
 
 class IMailboxFoldersByContainer(BaseEndpoint):
     def __init__(self, apiKey, url, container):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mail_folders_container/{container}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/IMailboxItems.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/IMailboxItems.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IMailboxItems_VERSION = "4.9.2928"
+IMailboxItems_VERSION = "4.9.2940"
 
 
 class IMailboxItems(BaseEndpoint):
     def __init__(self, apiKey, url, replicatedMailboxUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mail_items/{replicatedMailboxUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/IOutbox.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/IOutbox.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IOutbox_VERSION = "4.9.2928"
+IOutbox_VERSION = "4.9.2940"
 
 
 class IOutbox(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid, mailboxUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/outbox/{domainUid}/{mailboxUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/IReadOnlyMailboxFolders.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/IReadOnlyMailboxFolders.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IReadOnlyMailboxFolders_VERSION = "4.9.2928"
+IReadOnlyMailboxFolders_VERSION = "4.9.2940"
 
 
 class IReadOnlyMailboxFolders(BaseEndpoint):
     def __init__(self, apiKey, url, container):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/db_replicated_mailboxes_folders/{container}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/IUserInbox.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/IUserInbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IUserInbox_VERSION = "4.9.2928"
+IUserInbox_VERSION = "4.9.2940"
 
 
 class IUserInbox(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid, userUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/inbox/{domainUid}/{userUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/ImapAck.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/ImapAck.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/ImapItemIdentifier.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/ImapItemIdentifier.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/ImportMailboxItemSet.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/ImportMailboxItemSet.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/ImportMailboxItemSetMailboxItemId.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/ImportMailboxItemSetMailboxItemId.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/ImportMailboxItemsStatus.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/ImportMailboxItemsStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/ImportMailboxItemsStatusImportStatus.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/ImportMailboxItemsStatusImportStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/ImportMailboxItemsStatusImportedMailboxItem.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/ImportMailboxItemsStatusImportedMailboxItem.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/MailboxFolder.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/MailboxFolder.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/MailboxFolderSearchQuery.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/MailboxFolderSearchQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/MailboxItem.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/MailboxItem.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/MessageBody.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/MessageBody.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/MessageBodyHeader.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/MessageBodyHeader.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/MessageBodyPart.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/MessageBodyPart.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/MessageBodyRecipient.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/MessageBodyRecipient.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/MessageBodyRecipientKind.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/MessageBodyRecipientKind.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/MessageSearchResult.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/MessageSearchResult.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/MessageSearchResultMbox.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/MessageSearchResultMbox.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/SearchQuery.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/SearchQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/SearchQueryFolderScope.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/SearchQueryFolderScope.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/SearchQueryHeader.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/SearchQueryHeader.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/SearchQueryHeaderQuery.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/SearchQueryHeaderQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/SearchQueryLogicalOperator.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/SearchQueryLogicalOperator.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/SearchQuerySearchScope.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/SearchQuerySearchScope.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/SearchResult.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/SearchResult.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/SearchSort.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/SearchSort.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/SearchSortOrder.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/SearchSortOrder.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/SearchSortSortCriteria.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/SearchSortSortCriteria.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/flags/ConversationFlagUpdate.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/flags/ConversationFlagUpdate.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/flags/FlagUpdate.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/flags/FlagUpdate.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/flags/ImportMailboxConversationSet.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/flags/ImportMailboxConversationSet.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/flags/MailboxItemFlag.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/flags/MailboxItemFlag.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/backend/mail/api/flags/MailboxItemFlagSystem.py` & `netbluemind4-4.9.2940/netbluemind/backend/mail/api/flags/MailboxItemFlagSystem.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/CalendarDescriptor.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/CalendarDescriptor.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/CalendarLookupResponse.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/CalendarLookupResponse.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/CalendarLookupResponseType.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/CalendarLookupResponseType.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/CalendarSettingsData.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/CalendarSettingsData.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/CalendarSettingsDataDay.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/CalendarSettingsDataDay.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/CalendarView.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/CalendarView.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/CalendarViewCalendarViewType.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/CalendarViewCalendarViewType.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/CalendarViewChanges.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/CalendarViewChanges.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/CalendarViewChangesItemAdd.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/CalendarViewChangesItemAdd.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/CalendarViewChangesItemDelete.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/CalendarViewChangesItemDelete.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/CalendarViewChangesItemModify.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/CalendarViewChangesItemModify.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/CalendarsVEventQuery.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/CalendarsVEventQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/ICalendar.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/ICalendar.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ICalendar_VERSION = "4.9.2928"
+ICalendar_VERSION = "4.9.2940"
 
 
 class ICalendar(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/calendars/{containerUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/ICalendarAutocomplete.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/ICalendarAutocomplete.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ICalendarAutocomplete_VERSION = "4.9.2928"
+ICalendarAutocomplete_VERSION = "4.9.2940"
 
 
 class ICalendarAutocomplete(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/calendar/autocomplete'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/ICalendarSettings.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/ICalendarSettings.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ICalendarSettings_VERSION = "4.9.2928"
+ICalendarSettings_VERSION = "4.9.2940"
 
 
 class ICalendarSettings(BaseEndpoint):
     def __init__(self, apiKey, url, calendarUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/calendars/{calendarUid}/_config'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/ICalendarUids.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/ICalendarUids.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ICalendarUids_VERSION = "4.9.2928"
+ICalendarUids_VERSION = "4.9.2940"
 
 
 class ICalendarUids(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/calendar/uids'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/ICalendarView.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/ICalendarView.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ICalendarView_VERSION = "4.9.2928"
+ICalendarView_VERSION = "4.9.2940"
 
 
 class ICalendarView(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/calendars/view/{containerUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/ICalendarViewUids.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/ICalendarViewUids.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ICalendarViewUids_VERSION = "4.9.2928"
+ICalendarViewUids_VERSION = "4.9.2940"
 
 
 class ICalendarViewUids(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/calendarview/uids'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/ICalendars.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/ICalendars.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ICalendars_VERSION = "4.9.2928"
+ICalendars_VERSION = "4.9.2940"
 
 
 class ICalendars(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/calendars'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/ICalendarsMgmt.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/ICalendarsMgmt.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ICalendarsMgmt_VERSION = "4.9.2928"
+ICalendarsMgmt_VERSION = "4.9.2940"
 
 
 class ICalendarsMgmt(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mgmt/calendars'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/IFreebusyMgmt.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/IFreebusyMgmt.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IFreebusyMgmt_VERSION = "4.9.2928"
+IFreebusyMgmt_VERSION = "4.9.2940"
 
 
 class IFreebusyMgmt(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mgmt/freebusy/{containerUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/IFreebusyUids.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/IFreebusyUids.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IFreebusyUids_VERSION = "4.9.2928"
+IFreebusyUids_VERSION = "4.9.2940"
 
 
 class IFreebusyUids(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/freebusy/uids'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/IPrint.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/IPrint.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IPrint_VERSION = "4.9.2928"
+IPrint_VERSION = "4.9.2940"
 
 
 class IPrint(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/calendars/print'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/IPublicFreebusy.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/IPublicFreebusy.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IPublicFreebusy_VERSION = "4.9.2928"
+IPublicFreebusy_VERSION = "4.9.2940"
 
 
 class IPublicFreebusy(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/calendars/sfreebusy'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/IPublishCalendar.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/IPublishCalendar.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IPublishCalendar_VERSION = "4.9.2928"
+IPublishCalendar_VERSION = "4.9.2940"
 
 
 class IPublishCalendar(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/calendars/publish/{containerUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/IUserCalendarViews.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/IUserCalendarViews.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IUserCalendarViews_VERSION = "4.9.2928"
+IUserCalendarViews_VERSION = "4.9.2940"
 
 
 class IUserCalendarViews(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid, userUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/users/{domainUid}/{userUid}/calendar-views'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/IVEvent.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/IVEvent.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IVEvent_VERSION = "4.9.2928"
+IVEvent_VERSION = "4.9.2940"
 
 
 class IVEvent(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/calendars/vevent/{containerUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/IVFreebusy.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/IVFreebusy.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IVFreebusy_VERSION = "4.9.2928"
+IVFreebusy_VERSION = "4.9.2940"
 
 
 class IVFreebusy(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/calendars/vfreebusy/{containerUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/PrintData.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/PrintData.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/PrintOptions.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/PrintOptions.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/PrintOptionsCalendarMetadata.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/PrintOptionsCalendarMetadata.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/PrintOptionsPrintFormat.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/PrintOptionsPrintFormat.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/PrintOptionsPrintLayout.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/PrintOptionsPrintLayout.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/PrintOptionsPrintView.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/PrintOptionsPrintView.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/PublishMode.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/PublishMode.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/VEvent.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/VEvent.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/VEventAttendeeQuery.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/VEventAttendeeQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/VEventChanges.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/VEventChanges.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/VEventChangesItemAdd.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/VEventChangesItemAdd.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/VEventChangesItemDelete.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/VEventChangesItemDelete.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/VEventChangesItemModify.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/VEventChangesItemModify.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/VEventCounter.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/VEventCounter.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/VEventCounterCounterOriginator.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/VEventCounterCounterOriginator.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/VEventOccurrence.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/VEventOccurrence.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/VEventQuery.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/VEventQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/VEventSeries.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/VEventSeries.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/VEventTransparency.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/VEventTransparency.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/VFreebusy.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/VFreebusy.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/VFreebusyQuery.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/VFreebusyQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/VFreebusySlot.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/VFreebusySlot.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/calendar/api/VFreebusyType.py` & `netbluemind4-4.9.2940/netbluemind/calendar/api/VFreebusyType.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/api/Email.py` & `netbluemind4-4.9.2940/netbluemind/core/api/Email.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/api/ImportStats.py` & `netbluemind4-4.9.2940/netbluemind/core/api/ImportStats.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/api/ListResult.py` & `netbluemind4-4.9.2940/netbluemind/core/api/ListResult.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/api/VersionInfo.py` & `netbluemind4-4.9.2940/netbluemind/core/api/VersionInfo.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/api/date/BmDateTime.py` & `netbluemind4-4.9.2940/netbluemind/core/api/date/BmDateTime.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/api/date/BmDateTimePrecision.py` & `netbluemind4-4.9.2940/netbluemind/core/api/date/BmDateTimePrecision.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/api/fault/ErrorCode.py` & `netbluemind4-4.9.2940/netbluemind/core/api/fault/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/api/Ack.py` & `netbluemind4-4.9.2940/netbluemind/core/container/api/Ack.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/api/ContainerHierarchyNode.py` & `netbluemind4-4.9.2940/netbluemind/core/container/api/ContainerHierarchyNode.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/api/ContainerQuery.py` & `netbluemind4-4.9.2940/netbluemind/core/container/api/ContainerQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/api/ContainerSubscription.py` & `netbluemind4-4.9.2940/netbluemind/core/container/api/ContainerSubscription.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/api/ContainerSubscriptionDescriptor.py` & `netbluemind4-4.9.2940/netbluemind/core/container/api/ContainerSubscriptionDescriptor.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/api/ContainerSubscriptionModel.py` & `netbluemind4-4.9.2940/netbluemind/core/container/api/ContainerSubscriptionModel.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/api/Count.py` & `netbluemind4-4.9.2940/netbluemind/core/container/api/Count.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/api/IChangelogSupport.py` & `netbluemind4-4.9.2940/netbluemind/core/container/api/IChangelogSupport.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IChangelogSupport_VERSION = "4.9.2928"
+IChangelogSupport_VERSION = "4.9.2940"
 
 
 class IChangelogSupport(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + ''
```

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/api/IContainerManagement.py` & `netbluemind4-4.9.2940/netbluemind/core/container/api/IContainerManagement.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IContainerManagement_VERSION = "4.9.2928"
+IContainerManagement_VERSION = "4.9.2940"
 
 
 class IContainerManagement(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/containers/_manage/{containerUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/api/IContainerSync.py` & `netbluemind4-4.9.2940/netbluemind/core/container/api/IContainerSync.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IContainerSync_VERSION = "4.9.2928"
+IContainerSync_VERSION = "4.9.2940"
 
 
 class IContainerSync(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/containers/_sync/{containerUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/api/IContainers.py` & `netbluemind4-4.9.2940/netbluemind/core/container/api/IContainers.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IContainers_VERSION = "4.9.2928"
+IContainers_VERSION = "4.9.2940"
 
 
 class IContainers(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/containers/_manage'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/api/IContainersFlatHierarchy.py` & `netbluemind4-4.9.2940/netbluemind/core/container/api/IContainersFlatHierarchy.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IContainersFlatHierarchy_VERSION = "4.9.2928"
+IContainersFlatHierarchy_VERSION = "4.9.2940"
 
 
 class IContainersFlatHierarchy(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid, ownerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/containers/_hierarchy/{domainUid}/{ownerUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/api/ICountingSupport.py` & `netbluemind4-4.9.2940/netbluemind/core/container/api/ICountingSupport.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ICountingSupport_VERSION = "4.9.2928"
+ICountingSupport_VERSION = "4.9.2940"
 
 
 class ICountingSupport(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + ''
```

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/api/IFlatHierarchyUids.py` & `netbluemind4-4.9.2940/netbluemind/core/container/api/IFlatHierarchyUids.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IFlatHierarchyUids_VERSION = "4.9.2928"
+IFlatHierarchyUids_VERSION = "4.9.2940"
 
 
 class IFlatHierarchyUids(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/flat_hierarchy/uids'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/api/IOfflineMgmt.py` & `netbluemind4-4.9.2940/netbluemind/core/container/api/IOfflineMgmt.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IOfflineMgmt_VERSION = "4.9.2928"
+IOfflineMgmt_VERSION = "4.9.2940"
 
 
 class IOfflineMgmt(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid, ownerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/offline/{domainUid}/{ownerUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/api/IOwnerSubscriptionUids.py` & `netbluemind4-4.9.2940/netbluemind/core/container/api/IOwnerSubscriptionUids.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IOwnerSubscriptionUids_VERSION = "4.9.2928"
+IOwnerSubscriptionUids_VERSION = "4.9.2940"
 
 
 class IOwnerSubscriptionUids(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/owner_subscriptions/uids'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/api/IOwnerSubscriptions.py` & `netbluemind4-4.9.2940/netbluemind/core/container/api/IOwnerSubscriptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IOwnerSubscriptions_VERSION = "4.9.2928"
+IOwnerSubscriptions_VERSION = "4.9.2940"
 
 
 class IOwnerSubscriptions(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid, ownerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/containers/_subscriptions/{domainUid}/{ownerUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/api/ISortingSupport.py` & `netbluemind4-4.9.2940/netbluemind/core/container/api/ISortingSupport.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ISortingSupport_VERSION = "4.9.2928"
+ISortingSupport_VERSION = "4.9.2940"
 
 
 class ISortingSupport(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + ''
```

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/api/IdRange.py` & `netbluemind4-4.9.2940/netbluemind/core/container/api/IdRange.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/BaseContainerDescriptor.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/BaseContainerDescriptor.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/ChangeLogEntry.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/ChangeLogEntry.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/ChangeLogEntryType.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/ChangeLogEntryType.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/ContainerChangelog.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/ContainerChangelog.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/ContainerChangeset.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/ContainerChangeset.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/ContainerDescriptor.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/ContainerDescriptor.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/ContainerModifiableDescriptor.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/ContainerModifiableDescriptor.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/ContainerSyncResult.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/ContainerSyncResult.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/ContainerSyncStatus.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/ContainerSyncStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/ContainerSyncStatusStatus.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/ContainerSyncStatusStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/ContainerUpdatesResult.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/ContainerUpdatesResult.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/ContainerUpdatesResultInError.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/ContainerUpdatesResultInError.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/IdQuery.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/IdQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/ItemChangeLogEntry.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/ItemChangeLogEntry.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/ItemChangelog.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/ItemChangelog.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/ItemContainerValue.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/ItemContainerValue.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/ItemDescriptor.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/ItemDescriptor.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/ItemFlag.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/ItemFlag.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/ItemFlagFilter.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/ItemFlagFilter.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/ItemIdentifier.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/ItemIdentifier.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/ItemUri.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/ItemUri.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/ItemValue.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/ItemValue.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/ItemVersion.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/ItemVersion.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/SortDescriptor.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/SortDescriptor.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/SortDescriptorDirection.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/SortDescriptorDirection.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/SortDescriptorField.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/SortDescriptorField.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/acl/AccessControlEntry.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/acl/AccessControlEntry.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/container/model/acl/Verb.py` & `netbluemind4-4.9.2940/netbluemind/core/container/model/acl/Verb.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/task/api/ITask.py` & `netbluemind4-4.9.2940/netbluemind/core/task/api/ITask.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ITask_VERSION = "4.9.2928"
+ITask_VERSION = "4.9.2940"
 
 
 class ITask(BaseEndpoint):
     def __init__(self, apiKey, url, taskId):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/tasks/{taskId}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/core/task/api/TaskRef.py` & `netbluemind4-4.9.2940/netbluemind/core/task/api/TaskRef.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/task/api/TaskStatus.py` & `netbluemind4-4.9.2940/netbluemind/core/task/api/TaskStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/core/task/api/TaskStatusState.py` & `netbluemind4-4.9.2940/netbluemind/core/task/api/TaskStatusState.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/cti/api/IComputerTelephonyIntegration.py` & `netbluemind4-4.9.2940/netbluemind/cti/api/IComputerTelephonyIntegration.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IComputerTelephonyIntegration_VERSION = "4.9.2928"
+IComputerTelephonyIntegration_VERSION = "4.9.2940"
 
 
 class IComputerTelephonyIntegration(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid, userUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/cti/{domainUid}/{userUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/cti/api/Status.py` & `netbluemind4-4.9.2940/netbluemind/cti/api/Status.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/cti/api/StatusPhoneState.py` & `netbluemind4-4.9.2940/netbluemind/cti/api/StatusPhoneState.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/cti/api/StatusType.py` & `netbluemind4-4.9.2940/netbluemind/cti/api/StatusType.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/dataprotect/api/DataProtectGeneration.py` & `netbluemind4-4.9.2940/netbluemind/dataprotect/api/DataProtectGeneration.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/dataprotect/api/GenerationContent.py` & `netbluemind4-4.9.2940/netbluemind/dataprotect/api/GenerationContent.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/dataprotect/api/GenerationStatus.py` & `netbluemind4-4.9.2940/netbluemind/dataprotect/api/GenerationStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/dataprotect/api/IDataProtect.py` & `netbluemind4-4.9.2940/netbluemind/dataprotect/api/IDataProtect.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IDataProtect_VERSION = "4.9.2928"
+IDataProtect_VERSION = "4.9.2940"
 
 
 class IDataProtect(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/dataprotect'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/dataprotect/api/PartGeneration.py` & `netbluemind4-4.9.2940/netbluemind/dataprotect/api/PartGeneration.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/dataprotect/api/Restorable.py` & `netbluemind4-4.9.2940/netbluemind/dataprotect/api/Restorable.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/dataprotect/api/RestorableKind.py` & `netbluemind4-4.9.2940/netbluemind/dataprotect/api/RestorableKind.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/dataprotect/api/RestoreDefinition.py` & `netbluemind4-4.9.2940/netbluemind/dataprotect/api/RestoreDefinition.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/dataprotect/api/RestoreOperation.py` & `netbluemind4-4.9.2940/netbluemind/dataprotect/api/RestoreOperation.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/dataprotect/api/RetentionPolicy.py` & `netbluemind4-4.9.2940/netbluemind/dataprotect/api/RetentionPolicy.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/device/api/Device.py` & `netbluemind4-4.9.2940/netbluemind/device/api/Device.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/device/api/IDevice.py` & `netbluemind4-4.9.2940/netbluemind/device/api/IDevice.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IDevice_VERSION = "4.9.2928"
+IDevice_VERSION = "4.9.2940"
 
 
 class IDevice(BaseEndpoint):
     def __init__(self, apiKey, url, userUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/devices/{userUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/device/api/IDeviceUids.py` & `netbluemind4-4.9.2940/netbluemind/device/api/IDeviceUids.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IDeviceUids_VERSION = "4.9.2928"
+IDeviceUids_VERSION = "4.9.2940"
 
 
 class IDeviceUids(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/device/uids'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/device/api/IDevices.py` & `netbluemind4-4.9.2940/netbluemind/device/api/IDevices.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IDevices_VERSION = "4.9.2928"
+IDevices_VERSION = "4.9.2940"
 
 
 class IDevices(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/devices'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/directory/api/BaseDirEntry.py` & `netbluemind4-4.9.2940/netbluemind/directory/api/BaseDirEntry.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/directory/api/BaseDirEntryAccountType.py` & `netbluemind4-4.9.2940/netbluemind/directory/api/BaseDirEntryAccountType.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/directory/api/BaseDirEntryKind.py` & `netbluemind4-4.9.2940/netbluemind/directory/api/BaseDirEntryKind.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/directory/api/DirBaseValue.py` & `netbluemind4-4.9.2940/netbluemind/directory/api/DirBaseValue.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/directory/api/DirEntry.py` & `netbluemind4-4.9.2940/netbluemind/directory/api/DirEntry.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/directory/api/DirEntryQuery.py` & `netbluemind4-4.9.2940/netbluemind/directory/api/DirEntryQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/directory/api/DirEntryQueryDir.py` & `netbluemind4-4.9.2940/netbluemind/directory/api/DirEntryQueryDir.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/directory/api/DirEntryQueryOrder.py` & `netbluemind4-4.9.2940/netbluemind/directory/api/DirEntryQueryOrder.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/directory/api/DirEntryQueryOrderBy.py` & `netbluemind4-4.9.2940/netbluemind/directory/api/DirEntryQueryOrderBy.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/directory/api/DirEntryQueryStateFilter.py` & `netbluemind4-4.9.2940/netbluemind/directory/api/DirEntryQueryStateFilter.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/directory/api/IDirEntryMaintenance.py` & `netbluemind4-4.9.2940/netbluemind/directory/api/IDirEntryMaintenance.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IDirEntryMaintenance_VERSION = "4.9.2928"
+IDirEntryMaintenance_VERSION = "4.9.2940"
 
 
 class IDirEntryMaintenance(BaseEndpoint):
     def __init__(self, apiKey, url, domain, entryUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/directory/{domain}/{entryUid}/mgmt'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/directory/api/IDirEntryPath.py` & `netbluemind4-4.9.2940/netbluemind/directory/api/IDirEntryPath.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IDirEntryPath_VERSION = "4.9.2928"
+IDirEntryPath_VERSION = "4.9.2940"
 
 
 class IDirEntryPath(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/directory/path'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/directory/api/IDirectory.py` & `netbluemind4-4.9.2940/netbluemind/directory/api/IDirectory.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IDirectory_VERSION = "4.9.2928"
+IDirectory_VERSION = "4.9.2940"
 
 
 class IDirectory(BaseEndpoint):
     def __init__(self, apiKey, url, domain):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/directory/{domain}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/directory/api/IOrgUnits.py` & `netbluemind4-4.9.2940/netbluemind/directory/api/IOrgUnits.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IOrgUnits_VERSION = "4.9.2928"
+IOrgUnits_VERSION = "4.9.2940"
 
 
 class IOrgUnits(BaseEndpoint):
     def __init__(self, apiKey, url, domain):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/directory/_ou/{domain}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/directory/api/MaintenanceOperation.py` & `netbluemind4-4.9.2940/netbluemind/directory/api/MaintenanceOperation.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/directory/api/OrgUnit.py` & `netbluemind4-4.9.2940/netbluemind/directory/api/OrgUnit.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/directory/api/OrgUnitPath.py` & `netbluemind4-4.9.2940/netbluemind/directory/api/OrgUnitPath.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/directory/api/OrgUnitQuery.py` & `netbluemind4-4.9.2940/netbluemind/directory/api/OrgUnitQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/directory/api/RepairConfig.py` & `netbluemind4-4.9.2940/netbluemind/directory/api/RepairConfig.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/document/api/Document.py` & `netbluemind4-4.9.2940/netbluemind/document/api/Document.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/document/api/DocumentMetadata.py` & `netbluemind4-4.9.2940/netbluemind/document/api/DocumentMetadata.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/document/api/IDocument.py` & `netbluemind4-4.9.2940/netbluemind/document/api/IDocument.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IDocument_VERSION = "4.9.2928"
+IDocument_VERSION = "4.9.2940"
 
 
 class IDocument(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid, itemUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/document/{containerUid}/{itemUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/documentfolder/api/DocumentFolder.py` & `netbluemind4-4.9.2940/netbluemind/documentfolder/api/DocumentFolder.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/documentfolder/api/IDocumentFolder.py` & `netbluemind4-4.9.2940/netbluemind/documentfolder/api/IDocumentFolder.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IDocumentFolder_VERSION = "4.9.2928"
+IDocumentFolder_VERSION = "4.9.2940"
 
 
 class IDocumentFolder(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/document/{containerUid}/'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/documentfolder/api/IDocumentFolderUids.py` & `netbluemind4-4.9.2940/netbluemind/documentfolder/api/IDocumentFolderUids.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IDocumentFolderUids_VERSION = "4.9.2928"
+IDocumentFolderUids_VERSION = "4.9.2940"
 
 
 class IDocumentFolderUids(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/document/uids'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/domain/api/Domain.py` & `netbluemind4-4.9.2940/netbluemind/domain/api/Domain.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/domain/api/IDomainSettings.py` & `netbluemind4-4.9.2940/netbluemind/domain/api/IDomainSettings.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IDomainSettings_VERSION = "4.9.2928"
+IDomainSettings_VERSION = "4.9.2940"
 
 
 class IDomainSettings(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/domains/{containerUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/domain/api/IDomains.py` & `netbluemind4-4.9.2940/netbluemind/domain/api/IDomains.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IDomains_VERSION = "4.9.2928"
+IDomains_VERSION = "4.9.2940"
 
 
 class IDomains(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/domains'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/eas/api/Account.py` & `netbluemind4-4.9.2940/netbluemind/eas/api/Account.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/eas/api/FolderSyncVersions.py` & `netbluemind4-4.9.2940/netbluemind/eas/api/FolderSyncVersions.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/eas/api/Heartbeat.py` & `netbluemind4-4.9.2940/netbluemind/eas/api/Heartbeat.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/eas/api/IEas.py` & `netbluemind4-4.9.2940/netbluemind/eas/api/IEas.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IEas_VERSION = "4.9.2928"
+IEas_VERSION = "4.9.2940"
 
 
 class IEas(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/eas'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/eas/api/SentItem.py` & `netbluemind4-4.9.2940/netbluemind/eas/api/SentItem.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/externaluser/api/ExternalUser.py` & `netbluemind4-4.9.2940/netbluemind/externaluser/api/ExternalUser.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/externaluser/api/IExternalUser.py` & `netbluemind4-4.9.2940/netbluemind/externaluser/api/IExternalUser.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IExternalUser_VERSION = "4.9.2928"
+IExternalUser_VERSION = "4.9.2940"
 
 
 class IExternalUser(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/externaluser/{domainUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/filehosting/api/Configuration.py` & `netbluemind4-4.9.2940/netbluemind/filehosting/api/Configuration.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/filehosting/api/FileHostingInfo.py` & `netbluemind4-4.9.2940/netbluemind/filehosting/api/FileHostingInfo.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/filehosting/api/FileHostingInfoType.py` & `netbluemind4-4.9.2940/netbluemind/filehosting/api/FileHostingInfoType.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/filehosting/api/FileHostingItem.py` & `netbluemind4-4.9.2940/netbluemind/filehosting/api/FileHostingItem.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/filehosting/api/FileHostingPublicLink.py` & `netbluemind4-4.9.2940/netbluemind/filehosting/api/FileHostingPublicLink.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/filehosting/api/FileType.py` & `netbluemind4-4.9.2940/netbluemind/filehosting/api/FileType.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/filehosting/api/IFileHosting.py` & `netbluemind4-4.9.2940/netbluemind/filehosting/api/IFileHosting.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IFileHosting_VERSION = "4.9.2928"
+IFileHosting_VERSION = "4.9.2940"
 
 
 class IFileHosting(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/filehosting/{domainUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/filehosting/api/IInternalBMFileSystem.py` & `netbluemind4-4.9.2940/netbluemind/filehosting/api/IInternalBMFileSystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IInternalBMFileSystem_VERSION = "4.9.2928"
+IInternalBMFileSystem_VERSION = "4.9.2940"
 
 
 class IInternalBMFileSystem(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/bmfilehosting'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/filehosting/api/Metadata.py` & `netbluemind4-4.9.2940/netbluemind/filehosting/api/Metadata.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/group/api/Group.py` & `netbluemind4-4.9.2940/netbluemind/group/api/Group.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/group/api/GroupSearchQuery.py` & `netbluemind4-4.9.2940/netbluemind/group/api/GroupSearchQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/group/api/IGroup.py` & `netbluemind4-4.9.2940/netbluemind/group/api/IGroup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IGroup_VERSION = "4.9.2928"
+IGroup_VERSION = "4.9.2940"
 
 
 class IGroup(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/groups/{domainUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/group/api/IGroupMember.py` & `netbluemind4-4.9.2940/netbluemind/group/api/IGroupMember.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IGroupMember_VERSION = "4.9.2928"
+IGroupMember_VERSION = "4.9.2940"
 
 
 class IGroupMember(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + ''
```

### Comparing `netbluemind4-4.9.2928/netbluemind/group/api/Member.py` & `netbluemind4-4.9.2940/netbluemind/group/api/Member.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/group/api/MemberType.py` & `netbluemind4-4.9.2940/netbluemind/group/api/MemberType.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/hsm/api/Demote.py` & `netbluemind4-4.9.2940/netbluemind/hsm/api/Demote.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/hsm/api/IHSM.py` & `netbluemind4-4.9.2940/netbluemind/hsm/api/IHSM.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IHSM_VERSION = "4.9.2928"
+IHSM_VERSION = "4.9.2940"
 
 
 class IHSM(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/hsm/{domainUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/hsm/api/Promote.py` & `netbluemind4-4.9.2940/netbluemind/hsm/api/Promote.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/hsm/api/TierChangeResult.py` & `netbluemind4-4.9.2940/netbluemind/hsm/api/TierChangeResult.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/icalendar/api/ICalendarElement.py` & `netbluemind4-4.9.2940/netbluemind/icalendar/api/ICalendarElement.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/icalendar/api/ICalendarElementAttendee.py` & `netbluemind4-4.9.2940/netbluemind/icalendar/api/ICalendarElementAttendee.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/icalendar/api/ICalendarElementCUType.py` & `netbluemind4-4.9.2940/netbluemind/icalendar/api/ICalendarElementCUType.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/icalendar/api/ICalendarElementClassification.py` & `netbluemind4-4.9.2940/netbluemind/icalendar/api/ICalendarElementClassification.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/icalendar/api/ICalendarElementOrganizer.py` & `netbluemind4-4.9.2940/netbluemind/icalendar/api/ICalendarElementOrganizer.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/icalendar/api/ICalendarElementParticipationStatus.py` & `netbluemind4-4.9.2940/netbluemind/icalendar/api/ICalendarElementParticipationStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/icalendar/api/ICalendarElementRRule.py` & `netbluemind4-4.9.2940/netbluemind/icalendar/api/ICalendarElementRRule.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/icalendar/api/ICalendarElementRRuleFrequency.py` & `netbluemind4-4.9.2940/netbluemind/icalendar/api/ICalendarElementRRuleFrequency.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/icalendar/api/ICalendarElementRRuleWeekDay.py` & `netbluemind4-4.9.2940/netbluemind/icalendar/api/ICalendarElementRRuleWeekDay.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/icalendar/api/ICalendarElementRole.py` & `netbluemind4-4.9.2940/netbluemind/icalendar/api/ICalendarElementRole.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/icalendar/api/ICalendarElementStatus.py` & `netbluemind4-4.9.2940/netbluemind/icalendar/api/ICalendarElementStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/icalendar/api/ICalendarElementVAlarm.py` & `netbluemind4-4.9.2940/netbluemind/icalendar/api/ICalendarElementVAlarm.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/icalendar/api/ICalendarElementVAlarmAction.py` & `netbluemind4-4.9.2940/netbluemind/icalendar/api/ICalendarElementVAlarmAction.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/im/api/IInstantMessaging.py` & `netbluemind4-4.9.2940/netbluemind/im/api/IInstantMessaging.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IInstantMessaging_VERSION = "4.9.2928"
+IInstantMessaging_VERSION = "4.9.2940"
 
 
 class IInstantMessaging(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/im'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/im/api/IMMessage.py` & `netbluemind4-4.9.2940/netbluemind/im/api/IMMessage.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailbox/api/IMailboxAclUids.py` & `netbluemind4-4.9.2940/netbluemind/mailbox/api/IMailboxAclUids.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IMailboxAclUids_VERSION = "4.9.2928"
+IMailboxAclUids_VERSION = "4.9.2940"
 
 
 class IMailboxAclUids(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mailbox/uids'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/mailbox/api/IMailboxMgmt.py` & `netbluemind4-4.9.2940/netbluemind/mailbox/api/IMailboxMgmt.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IMailboxMgmt_VERSION = "4.9.2928"
+IMailboxMgmt_VERSION = "4.9.2940"
 
 
 class IMailboxMgmt(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mgmt/mailbox/{domainUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/mailbox/api/IMailboxes.py` & `netbluemind4-4.9.2940/netbluemind/mailbox/api/IMailboxes.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IMailboxes_VERSION = "4.9.2928"
+IMailboxes_VERSION = "4.9.2940"
 
 
 class IMailboxes(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mailboxes/{domainUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/mailbox/api/MailFilter.py` & `netbluemind4-4.9.2940/netbluemind/mailbox/api/MailFilter.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailbox/api/MailFilterForwarding.py` & `netbluemind4-4.9.2940/netbluemind/mailbox/api/MailFilterForwarding.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailbox/api/MailFilterRule.py` & `netbluemind4-4.9.2940/netbluemind/mailbox/api/MailFilterRule.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailbox/api/MailFilterVacation.py` & `netbluemind4-4.9.2940/netbluemind/mailbox/api/MailFilterVacation.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailbox/api/Mailbox.py` & `netbluemind4-4.9.2940/netbluemind/mailbox/api/Mailbox.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailbox/api/MailboxConfig.py` & `netbluemind4-4.9.2940/netbluemind/mailbox/api/MailboxConfig.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailbox/api/MailboxQuota.py` & `netbluemind4-4.9.2940/netbluemind/mailbox/api/MailboxQuota.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailbox/api/MailboxRouting.py` & `netbluemind4-4.9.2940/netbluemind/mailbox/api/MailboxRouting.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailbox/api/MailboxType.py` & `netbluemind4-4.9.2940/netbluemind/mailbox/api/MailboxType.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailbox/api/ShardStats.py` & `netbluemind4-4.9.2940/netbluemind/mailbox/api/ShardStats.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailbox/api/ShardStatsMailboxStats.py` & `netbluemind4-4.9.2940/netbluemind/mailbox/api/ShardStatsMailboxStats.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailbox/api/ShardStatsState.py` & `netbluemind4-4.9.2940/netbluemind/mailbox/api/ShardStatsState.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailbox/api/SimpleShardStats.py` & `netbluemind4-4.9.2940/netbluemind/mailbox/api/SimpleShardStats.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailbox/identity/api/IMailboxIdentity.py` & `netbluemind4-4.9.2940/netbluemind/mailbox/identity/api/IMailboxIdentity.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IMailboxIdentity_VERSION = "4.9.2928"
+IMailboxIdentity_VERSION = "4.9.2940"
 
 
 class IMailboxIdentity(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid, mboxUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mailboxes/{domainUid}/identity/{mboxUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/mailbox/identity/api/Identity.py` & `netbluemind4-4.9.2940/netbluemind/mailbox/identity/api/Identity.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailbox/identity/api/IdentityDescription.py` & `netbluemind4-4.9.2940/netbluemind/mailbox/identity/api/IdentityDescription.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailbox/identity/api/SignatureFormat.py` & `netbluemind4-4.9.2940/netbluemind/mailbox/identity/api/SignatureFormat.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailflow/common/api/AssignmentActionMapping.py` & `netbluemind4-4.9.2940/netbluemind/mailflow/common/api/AssignmentActionMapping.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailflow/common/api/Message.py` & `netbluemind4-4.9.2940/netbluemind/mailflow/common/api/Message.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailflow/common/api/Recipient.py` & `netbluemind4-4.9.2940/netbluemind/mailflow/common/api/Recipient.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailflow/common/api/RecipientAddressType.py` & `netbluemind4-4.9.2940/netbluemind/mailflow/common/api/RecipientAddressType.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailflow/common/api/RecipientRecipientType.py` & `netbluemind4-4.9.2940/netbluemind/mailflow/common/api/RecipientRecipientType.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailflow/common/api/SendingAs.py` & `netbluemind4-4.9.2940/netbluemind/mailflow/common/api/SendingAs.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailmessage/api/IMailTip.py` & `netbluemind4-4.9.2940/netbluemind/mailmessage/api/IMailTip.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IMailTip_VERSION = "4.9.2928"
+IMailTip_VERSION = "4.9.2940"
 
 
 class IMailTip(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mailtip/{domainUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/mailmessage/api/MailTip.py` & `netbluemind4-4.9.2940/netbluemind/mailmessage/api/MailTip.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailmessage/api/MailTipContext.py` & `netbluemind4-4.9.2940/netbluemind/mailmessage/api/MailTipContext.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailmessage/api/MailTipFilter.py` & `netbluemind4-4.9.2940/netbluemind/mailmessage/api/MailTipFilter.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailmessage/api/MailTipFilterFilterType.py` & `netbluemind4-4.9.2940/netbluemind/mailmessage/api/MailTipFilterFilterType.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailmessage/api/MailTips.py` & `netbluemind4-4.9.2940/netbluemind/mailmessage/api/MailTips.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailmessage/api/MessageContext.py` & `netbluemind4-4.9.2940/netbluemind/mailmessage/api/MessageContext.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/mailshare/api/IMailshare.py` & `netbluemind4-4.9.2940/netbluemind/mailshare/api/IMailshare.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IMailshare_VERSION = "4.9.2928"
+IMailshare_VERSION = "4.9.2940"
 
 
 class IMailshare(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mailshares/{domainUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/mailshare/api/Mailshare.py` & `netbluemind4-4.9.2940/netbluemind/mailshare/api/Mailshare.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/notes/api/INote.py` & `netbluemind4-4.9.2940/netbluemind/notes/api/INote.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-INote_VERSION = "4.9.2928"
+INote_VERSION = "4.9.2940"
 
 
 class INote(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/notes/{containerUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/notes/api/INoteIndexMgmt.py` & `netbluemind4-4.9.2940/netbluemind/notes/api/INoteIndexMgmt.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-INoteIndexMgmt_VERSION = "4.9.2928"
+INoteIndexMgmt_VERSION = "4.9.2940"
 
 
 class INoteIndexMgmt(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mgmt/notes'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/notes/api/INoteUids.py` & `netbluemind4-4.9.2940/netbluemind/notes/api/INoteUids.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-INoteUids_VERSION = "4.9.2928"
+INoteUids_VERSION = "4.9.2940"
 
 
 class INoteUids(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/notes/uids'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/notes/api/INotes.py` & `netbluemind4-4.9.2940/netbluemind/notes/api/INotes.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-INotes_VERSION = "4.9.2928"
+INotes_VERSION = "4.9.2940"
 
 
 class INotes(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/notes'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/notes/api/VNote.py` & `netbluemind4-4.9.2940/netbluemind/notes/api/VNote.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/notes/api/VNoteChanges.py` & `netbluemind4-4.9.2940/netbluemind/notes/api/VNoteChanges.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/notes/api/VNoteChangesItemAdd.py` & `netbluemind4-4.9.2940/netbluemind/notes/api/VNoteChangesItemAdd.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/notes/api/VNoteChangesItemDelete.py` & `netbluemind4-4.9.2940/netbluemind/notes/api/VNoteChangesItemDelete.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/notes/api/VNoteChangesItemModify.py` & `netbluemind4-4.9.2940/netbluemind/notes/api/VNoteChangesItemModify.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/notes/api/VNoteColor.py` & `netbluemind4-4.9.2940/netbluemind/notes/api/VNoteColor.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/notes/api/VNoteQuery.py` & `netbluemind4-4.9.2940/netbluemind/notes/api/VNoteQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/notes/api/VNotesQuery.py` & `netbluemind4-4.9.2940/netbluemind/notes/api/VNotesQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/python/client.py` & `netbluemind4-4.9.2940/netbluemind/python/client.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/python/serder.py` & `netbluemind4-4.9.2940/netbluemind/python/serder.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/resource/api/EventInfo.py` & `netbluemind4-4.9.2940/netbluemind/resource/api/EventInfo.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/resource/api/IResources.py` & `netbluemind4-4.9.2940/netbluemind/resource/api/IResources.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IResources_VERSION = "4.9.2928"
+IResources_VERSION = "4.9.2940"
 
 
 class IResources(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/resources/{domainUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/resource/api/ResourceDescriptor.py` & `netbluemind4-4.9.2940/netbluemind/resource/api/ResourceDescriptor.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/resource/api/ResourceDescriptorPropertyValue.py` & `netbluemind4-4.9.2940/netbluemind/resource/api/ResourceDescriptorPropertyValue.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/resource/api/ResourceReservationMode.py` & `netbluemind4-4.9.2940/netbluemind/resource/api/ResourceReservationMode.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/resource/api/type/IResourceTypeUids.py` & `netbluemind4-4.9.2940/netbluemind/resource/api/type/IResourceTypeUids.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IResourceTypeUids_VERSION = "4.9.2928"
+IResourceTypeUids_VERSION = "4.9.2940"
 
 
 class IResourceTypeUids(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mailbox/uids'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/resource/api/type/IResourceTypes.py` & `netbluemind4-4.9.2940/netbluemind/resource/api/type/IResourceTypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IResourceTypes_VERSION = "4.9.2928"
+IResourceTypes_VERSION = "4.9.2940"
 
 
 class IResourceTypes(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/resources/{domainUid}/type'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/resource/api/type/ResourceType.py` & `netbluemind4-4.9.2940/netbluemind/resource/api/type/ResourceType.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/resource/api/type/ResourceTypeDescriptor.py` & `netbluemind4-4.9.2940/netbluemind/resource/api/type/ResourceTypeDescriptor.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/resource/api/type/ResourceTypeDescriptorProperty.py` & `netbluemind4-4.9.2940/netbluemind/resource/api/type/ResourceTypeDescriptorProperty.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/resource/api/type/ResourceTypeDescriptorPropertyType.py` & `netbluemind4-4.9.2940/netbluemind/resource/api/type/ResourceTypeDescriptorPropertyType.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/role/api/IRoles.py` & `netbluemind4-4.9.2940/netbluemind/role/api/IRoles.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IRoles_VERSION = "4.9.2928"
+IRoles_VERSION = "4.9.2940"
 
 
 class IRoles(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/roles'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/role/api/RoleDescriptor.py` & `netbluemind4-4.9.2940/netbluemind/role/api/RoleDescriptor.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/role/api/RolesCategory.py` & `netbluemind4-4.9.2940/netbluemind/role/api/RolesCategory.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/scheduledjob/api/IJob.py` & `netbluemind4-4.9.2940/netbluemind/scheduledjob/api/IJob.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IJob_VERSION = "4.9.2928"
+IJob_VERSION = "4.9.2940"
 
 
 class IJob(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/scheduledjobs'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/scheduledjob/api/Job.py` & `netbluemind4-4.9.2940/netbluemind/scheduledjob/api/Job.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/scheduledjob/api/JobDomainStatus.py` & `netbluemind4-4.9.2940/netbluemind/scheduledjob/api/JobDomainStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/scheduledjob/api/JobExecution.py` & `netbluemind4-4.9.2940/netbluemind/scheduledjob/api/JobExecution.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/scheduledjob/api/JobExecutionQuery.py` & `netbluemind4-4.9.2940/netbluemind/scheduledjob/api/JobExecutionQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/scheduledjob/api/JobExitStatus.py` & `netbluemind4-4.9.2940/netbluemind/scheduledjob/api/JobExitStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/scheduledjob/api/JobKind.py` & `netbluemind4-4.9.2940/netbluemind/scheduledjob/api/JobKind.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/scheduledjob/api/JobPlanification.py` & `netbluemind4-4.9.2940/netbluemind/scheduledjob/api/JobPlanification.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/scheduledjob/api/JobQuery.py` & `netbluemind4-4.9.2940/netbluemind/scheduledjob/api/JobQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/scheduledjob/api/JobRec.py` & `netbluemind4-4.9.2940/netbluemind/scheduledjob/api/JobRec.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/scheduledjob/api/LogEntry.py` & `netbluemind4-4.9.2940/netbluemind/scheduledjob/api/LogEntry.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/scheduledjob/api/LogLevel.py` & `netbluemind4-4.9.2940/netbluemind/scheduledjob/api/LogLevel.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/scheduledjob/api/PlanKind.py` & `netbluemind4-4.9.2940/netbluemind/scheduledjob/api/PlanKind.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/server/api/Assignment.py` & `netbluemind4-4.9.2940/netbluemind/server/api/Assignment.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/server/api/CommandStatus.py` & `netbluemind4-4.9.2940/netbluemind/server/api/CommandStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/server/api/IServer.py` & `netbluemind4-4.9.2940/netbluemind/server/api/IServer.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IServer_VERSION = "4.9.2928"
+IServer_VERSION = "4.9.2940"
 
 
 class IServer(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/servers/{containerUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/server/api/Server.py` & `netbluemind4-4.9.2940/netbluemind/server/api/Server.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/CertData.py` & `netbluemind4-4.9.2940/netbluemind/system/api/CertData.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/CertDataCertificateDomainEngine.py` & `netbluemind4-4.9.2940/netbluemind/system/api/CertDataCertificateDomainEngine.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/CloneConfiguration.py` & `netbluemind4-4.9.2940/netbluemind/system/api/CloneConfiguration.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/CloneConfigurationMode.py` & `netbluemind4-4.9.2940/netbluemind/system/api/CloneConfigurationMode.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/ConnectionTestStatus.py` & `netbluemind4-4.9.2940/netbluemind/system/api/ConnectionTestStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/CustomLogo.py` & `netbluemind4-4.9.2940/netbluemind/system/api/CustomLogo.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/DomainTemplate.py` & `netbluemind4-4.9.2940/netbluemind/system/api/DomainTemplate.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/DomainTemplateDescription.py` & `netbluemind4-4.9.2940/netbluemind/system/api/DomainTemplateDescription.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/DomainTemplateDescriptionI18NDescription.py` & `netbluemind4-4.9.2940/netbluemind/system/api/DomainTemplateDescriptionI18NDescription.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/DomainTemplateKind.py` & `netbluemind4-4.9.2940/netbluemind/system/api/DomainTemplateKind.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/DomainTemplateTag.py` & `netbluemind4-4.9.2940/netbluemind/system/api/DomainTemplateTag.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/ExternalSystem.py` & `netbluemind4-4.9.2940/netbluemind/system/api/ExternalSystem.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/ExternalSystemAuthKind.py` & `netbluemind4-4.9.2940/netbluemind/system/api/ExternalSystemAuthKind.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/ICacheMgmt.py` & `netbluemind4-4.9.2940/netbluemind/system/api/ICacheMgmt.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ICacheMgmt_VERSION = "4.9.2928"
+ICacheMgmt_VERSION = "4.9.2940"
 
 
 class ICacheMgmt(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/system/cache'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/ICustomTheme.py` & `netbluemind4-4.9.2940/netbluemind/system/api/ICustomTheme.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ICustomTheme_VERSION = "4.9.2928"
+ICustomTheme_VERSION = "4.9.2940"
 
 
 class ICustomTheme(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + ''
```

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/IDomainTemplate.py` & `netbluemind4-4.9.2940/netbluemind/system/api/IDomainTemplate.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IDomainTemplate_VERSION = "4.9.2928"
+IDomainTemplate_VERSION = "4.9.2940"
 
 
 class IDomainTemplate(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/system/domaintemplate'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/IExternalSystem.py` & `netbluemind4-4.9.2940/netbluemind/system/api/IExternalSystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IExternalSystem_VERSION = "4.9.2928"
+IExternalSystem_VERSION = "4.9.2940"
 
 
 class IExternalSystem(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/system/external'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/IGlobalSettings.py` & `netbluemind4-4.9.2940/netbluemind/system/api/IGlobalSettings.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IGlobalSettings_VERSION = "4.9.2928"
+IGlobalSettings_VERSION = "4.9.2940"
 
 
 class IGlobalSettings(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/global_settings'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/IInstallation.py` & `netbluemind4-4.9.2940/netbluemind/system/api/IInstallation.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IInstallation_VERSION = "4.9.2928"
+IInstallation_VERSION = "4.9.2940"
 
 
 class IInstallation(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/system/installation'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/IMailDeliveryMgmt.py` & `netbluemind4-4.9.2940/netbluemind/system/api/IMailDeliveryMgmt.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IMailDeliveryMgmt_VERSION = "4.9.2928"
+IMailDeliveryMgmt_VERSION = "4.9.2940"
 
 
 class IMailDeliveryMgmt(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/system/maildelivery/mgmt'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/ISchemaMgmt.py` & `netbluemind4-4.9.2940/netbluemind/system/api/ISchemaMgmt.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ISchemaMgmt_VERSION = "4.9.2928"
+ISchemaMgmt_VERSION = "4.9.2940"
 
 
 class ISchemaMgmt(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mgmt/schema'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/ISecurityMgmt.py` & `netbluemind4-4.9.2940/netbluemind/system/api/ISecurityMgmt.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ISecurityMgmt_VERSION = "4.9.2928"
+ISecurityMgmt_VERSION = "4.9.2940"
 
 
 class ISecurityMgmt(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/system/security'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/ISystemConfiguration.py` & `netbluemind4-4.9.2940/netbluemind/system/api/ISystemConfiguration.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ISystemConfiguration_VERSION = "4.9.2928"
+ISystemConfiguration_VERSION = "4.9.2940"
 
 
 class ISystemConfiguration(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/configuration'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/InstallationVersion.py` & `netbluemind4-4.9.2940/netbluemind/system/api/InstallationVersion.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/PublicInfos.py` & `netbluemind4-4.9.2940/netbluemind/system/api/PublicInfos.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/SchemaCheckInfo.py` & `netbluemind4-4.9.2940/netbluemind/system/api/SchemaCheckInfo.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/SubscriptionInformations.py` & `netbluemind4-4.9.2940/netbluemind/system/api/SubscriptionInformations.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/SubscriptionInformationsInstallationIndicator.py` & `netbluemind4-4.9.2940/netbluemind/system/api/SubscriptionInformationsInstallationIndicator.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/SubscriptionInformationsInstallationIndicatorKind.py` & `netbluemind4-4.9.2940/netbluemind/system/api/SubscriptionInformationsInstallationIndicatorKind.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/SubscriptionInformationsKind.py` & `netbluemind4-4.9.2940/netbluemind/system/api/SubscriptionInformationsKind.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/SubscriptionInformationsMessage.py` & `netbluemind4-4.9.2940/netbluemind/system/api/SubscriptionInformationsMessage.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/SubscriptionInformationsMessageCode.py` & `netbluemind4-4.9.2940/netbluemind/system/api/SubscriptionInformationsMessageCode.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/SubscriptionInformationsMessageKind.py` & `netbluemind4-4.9.2940/netbluemind/system/api/SubscriptionInformationsMessageKind.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/SystemConf.py` & `netbluemind4-4.9.2940/netbluemind/system/api/SystemConf.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/SystemState.py` & `netbluemind4-4.9.2940/netbluemind/system/api/SystemState.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/UpgradeReport.py` & `netbluemind4-4.9.2940/netbluemind/system/api/UpgradeReport.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/UpgradeReportStatus.py` & `netbluemind4-4.9.2940/netbluemind/system/api/UpgradeReportStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/UpgradeReportUpgraderReport.py` & `netbluemind4-4.9.2940/netbluemind/system/api/UpgradeReportUpgraderReport.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/UpgradeStatus.py` & `netbluemind4-4.9.2940/netbluemind/system/api/UpgradeStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/UpgradeStatusState.py` & `netbluemind4-4.9.2940/netbluemind/system/api/UpgradeStatusState.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/hot/upgrade/HotUpgradeProgress.py` & `netbluemind4-4.9.2940/netbluemind/system/api/hot/upgrade/HotUpgradeProgress.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/hot/upgrade/HotUpgradeTask.py` & `netbluemind4-4.9.2940/netbluemind/system/api/hot/upgrade/HotUpgradeTask.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/hot/upgrade/HotUpgradeTaskExecutionMode.py` & `netbluemind4-4.9.2940/netbluemind/system/api/hot/upgrade/HotUpgradeTaskExecutionMode.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/hot/upgrade/HotUpgradeTaskFilter.py` & `netbluemind4-4.9.2940/netbluemind/system/api/hot/upgrade/HotUpgradeTaskFilter.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/hot/upgrade/HotUpgradeTaskStatus.py` & `netbluemind4-4.9.2940/netbluemind/system/api/hot/upgrade/HotUpgradeTaskStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/hot/upgrade/IHotUpgrade.py` & `netbluemind4-4.9.2940/netbluemind/system/api/hot/upgrade/IHotUpgrade.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IHotUpgrade_VERSION = "4.9.2928"
+IHotUpgrade_VERSION = "4.9.2940"
 
 
 class IHotUpgrade(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/hot_upgrade'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/system/api/hot/upgrade/IInternalHotUpgrade.py` & `netbluemind4-4.9.2940/netbluemind/system/api/hot/upgrade/IInternalHotUpgrade.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IInternalHotUpgrade_VERSION = "4.9.2928"
+IInternalHotUpgrade_VERSION = "4.9.2940"
 
 
 class IInternalHotUpgrade(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/hot_upgrade'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/tag/api/ITagUids.py` & `netbluemind4-4.9.2940/netbluemind/tag/api/ITagUids.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ITagUids_VERSION = "4.9.2928"
+ITagUids_VERSION = "4.9.2940"
 
 
 class ITagUids(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/tags/uids'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/tag/api/ITags.py` & `netbluemind4-4.9.2940/netbluemind/tag/api/ITags.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ITags_VERSION = "4.9.2928"
+ITags_VERSION = "4.9.2940"
 
 
 class ITags(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/tags/{containerUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/tag/api/Tag.py` & `netbluemind4-4.9.2940/netbluemind/tag/api/Tag.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/tag/api/TagChanges.py` & `netbluemind4-4.9.2940/netbluemind/tag/api/TagChanges.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/tag/api/TagChangesItemAdd.py` & `netbluemind4-4.9.2940/netbluemind/tag/api/TagChangesItemAdd.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/tag/api/TagChangesItemDelete.py` & `netbluemind4-4.9.2940/netbluemind/tag/api/TagChangesItemDelete.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/tag/api/TagChangesItemModify.py` & `netbluemind4-4.9.2940/netbluemind/tag/api/TagChangesItemModify.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/tag/api/TagRef.py` & `netbluemind4-4.9.2940/netbluemind/tag/api/TagRef.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/todolist/api/ITodoList.py` & `netbluemind4-4.9.2940/netbluemind/todolist/api/ITodoList.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ITodoList_VERSION = "4.9.2928"
+ITodoList_VERSION = "4.9.2940"
 
 
 class ITodoList(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/todolist/{containerUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/todolist/api/ITodoLists.py` & `netbluemind4-4.9.2940/netbluemind/todolist/api/ITodoLists.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ITodoLists_VERSION = "4.9.2928"
+ITodoLists_VERSION = "4.9.2940"
 
 
 class ITodoLists(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/todolists'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/todolist/api/ITodoListsMgmt.py` & `netbluemind4-4.9.2940/netbluemind/todolist/api/ITodoListsMgmt.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ITodoListsMgmt_VERSION = "4.9.2928"
+ITodoListsMgmt_VERSION = "4.9.2940"
 
 
 class ITodoListsMgmt(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mgmt/todolists'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/todolist/api/ITodoUids.py` & `netbluemind4-4.9.2940/netbluemind/todolist/api/ITodoUids.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ITodoUids_VERSION = "4.9.2928"
+ITodoUids_VERSION = "4.9.2940"
 
 
 class ITodoUids(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/todolist/uids'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/todolist/api/IVTodo.py` & `netbluemind4-4.9.2940/netbluemind/todolist/api/IVTodo.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IVTodo_VERSION = "4.9.2928"
+IVTodo_VERSION = "4.9.2940"
 
 
 class IVTodo(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/todolists/vtodos/{containerUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/todolist/api/TodoListsVTodoQuery.py` & `netbluemind4-4.9.2940/netbluemind/todolist/api/TodoListsVTodoQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/todolist/api/VTodo.py` & `netbluemind4-4.9.2940/netbluemind/todolist/api/VTodo.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/todolist/api/VTodoChanges.py` & `netbluemind4-4.9.2940/netbluemind/todolist/api/VTodoChanges.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/todolist/api/VTodoChangesItemAdd.py` & `netbluemind4-4.9.2940/netbluemind/todolist/api/VTodoChangesItemAdd.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/todolist/api/VTodoChangesItemDelete.py` & `netbluemind4-4.9.2940/netbluemind/todolist/api/VTodoChangesItemDelete.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/todolist/api/VTodoChangesItemModify.py` & `netbluemind4-4.9.2940/netbluemind/todolist/api/VTodoChangesItemModify.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/todolist/api/VTodoQuery.py` & `netbluemind4-4.9.2940/netbluemind/todolist/api/VTodoQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/user/api/ChangePassword.py` & `netbluemind4-4.9.2940/netbluemind/user/api/ChangePassword.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/user/api/IUser.py` & `netbluemind4-4.9.2940/netbluemind/user/api/IUser.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IUser_VERSION = "4.9.2928"
+IUser_VERSION = "4.9.2940"
 
 
 class IUser(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/users/{domainUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/user/api/IUserExternalAccount.py` & `netbluemind4-4.9.2940/netbluemind/user/api/IUserExternalAccount.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IUserExternalAccount_VERSION = "4.9.2928"
+IUserExternalAccount_VERSION = "4.9.2940"
 
 
 class IUserExternalAccount(BaseEndpoint):
     def __init__(self, apiKey, url, domain, uid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/users/{domain}/{uid}/accounts'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/user/api/IUserMailIdentities.py` & `netbluemind4-4.9.2940/netbluemind/user/api/IUserMailIdentities.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IUserMailIdentities_VERSION = "4.9.2928"
+IUserMailIdentities_VERSION = "4.9.2940"
 
 
 class IUserMailIdentities(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid, userUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/users/{domainUid}/{userUid}/identity'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/user/api/IUserSettings.py` & `netbluemind4-4.9.2940/netbluemind/user/api/IUserSettings.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IUserSettings_VERSION = "4.9.2928"
+IUserSettings_VERSION = "4.9.2940"
 
 
 class IUserSettings(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/users/{containerUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/user/api/IUserSubscription.py` & `netbluemind4-4.9.2940/netbluemind/user/api/IUserSubscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IUserSubscription_VERSION = "4.9.2928"
+IUserSubscription_VERSION = "4.9.2940"
 
 
 class IUserSubscription(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/users/{domainUid}/subscriptions'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/user/api/User.py` & `netbluemind4-4.9.2940/netbluemind/user/api/User.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/user/api/UserAccount.py` & `netbluemind4-4.9.2940/netbluemind/user/api/UserAccount.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/user/api/UserAccountInfo.py` & `netbluemind4-4.9.2940/netbluemind/user/api/UserAccountInfo.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/user/api/UserMailIdentity.py` & `netbluemind4-4.9.2940/netbluemind/user/api/UserMailIdentity.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/user/api/UserSettings.py` & `netbluemind4-4.9.2940/netbluemind/user/api/UserSettings.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind/webappdata/api/IWebAppData.py` & `netbluemind4-4.9.2940/netbluemind/webappdata/api/IWebAppData.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IWebAppData_VERSION = "4.9.2928"
+IWebAppData_VERSION = "4.9.2940"
 
 
 class IWebAppData(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/webappdata/{containerUid}'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/webappdata/api/IWebAppDataUids.py` & `netbluemind4-4.9.2940/netbluemind/webappdata/api/IWebAppDataUids.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IWebAppDataUids_VERSION = "4.9.2928"
+IWebAppDataUids_VERSION = "4.9.2940"
 
 
 class IWebAppDataUids(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/webappdata/uids'
```

### Comparing `netbluemind4-4.9.2928/netbluemind/webappdata/api/WebAppData.py` & `netbluemind4-4.9.2940/netbluemind/webappdata/api/WebAppData.py`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/netbluemind4.egg-info/PKG-INFO` & `netbluemind4-4.9.2940/netbluemind4.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbluemind4
-Version: 4.9.2928
+Version: 4.9.2940
 Summary: Automatically generated client for BlueMind >= 4 REST API. Check netbluemind for older releases
 Home-page: http://git.blue-mind.net/bluemind/
 Author: BlueMind team
 Author-email: contact@bluemind.net
 Keywords: bluemind,rest,api,mail,groupware
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `netbluemind4-4.9.2928/netbluemind4.egg-info/SOURCES.txt` & `netbluemind4-4.9.2940/netbluemind4.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbluemind4-4.9.2928/setup.py` & `netbluemind4-4.9.2940/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 install_requires = ['requests']
 if sys.version_info < (3, 4):
     install_requires.append('enum34')
 
 setup(
     name = 'netbluemind4',
     packages = find_packages(),
-    version = '4.9.2928',
+    version = '4.9.2940',
     description = 'Automatically generated client for BlueMind >= 4 REST API. Check netbluemind for older releases',
     author = 'BlueMind team',
     author_email = 'contact@bluemind.net',
     url = 'http://git.blue-mind.net/bluemind/',
     keywords = ['bluemind', 'rest', 'api', 'mail', 'groupware'],
     classifiers = [
         'Development Status :: 5 - Production/Stable',
```

