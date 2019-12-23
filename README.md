# ![LOGO](logo.png) Slack Web API **flow**ground Connector

## Description

A generated **flow**ground connector for the Slack Web API API (version 1.2.0).

Generated from: https://slack.com/api<br/>
Generated at: 2019-12-23T14:13:15+00:00

## API Description

One way to interact with the Slack platform is its HTTP RPC-based Web API, a collection of methods requiring OAuth 2.0-based user, bot, or workspace tokens blessed with related OAuth scopes.<br/>

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### admin_users_session_reset
> Wipes all valid sessions on all devices for a given user<br/>

*Tags:* `admin.users.session` `admin`

### api_test
> Checks API calling code.<br/>

*Tags:* `api`

#### Input Parameters
* `foo` - _optional_ - example property to return<br/>
* `error` - _optional_ - Error response to return<br/>

### apps_permissions_info
> Returns list of permissions this app has on a team.<br/>

*Tags:* `apps.permissions` `apps`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `none`<br/>

### apps_permissions_request
> Allows an app to request additional scopes<br/>

*Tags:* `apps.permissions` `apps`

#### Input Parameters
* `scopes` - _optional_ - A comma separated list of scopes to request for<br/>
* `token` - _optional_ - Authentication token. Requires scope: `none`<br/>
* `trigger_id` - _optional_ - Token used to trigger the permissions API<br/>

### apps_permissions_resources_list
> Returns list of resource grants this app has on a team.<br/>

*Tags:* `apps.permissions.resources` `apps`

#### Input Parameters
* `cursor` - _optional_ - Paginate through collections of data by setting the `cursor` parameter to a `next_cursor` attribute returned by a previous request's `response_metadata`. Default value fetches the first "page" of the collection. See [pagination](/docs/pagination) for more detail.<br/>
* `token` - _optional_ - Authentication token. Requires scope: `none`<br/>
* `limit` - _optional_ - The maximum number of items to return.<br/>

### apps_permissions_scopes_list
> Returns list of scopes this app has on a team.<br/>

*Tags:* `apps.permissions.scopes` `apps`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `none`<br/>

### apps_permissions_users_list
> Returns list of user grants and corresponding scopes this app has on a team.<br/>

*Tags:* `apps.permissions.users` `apps`

#### Input Parameters
* `cursor` - _optional_ - Paginate through collections of data by setting the `cursor` parameter to a `next_cursor` attribute returned by a previous request's `response_metadata`. Default value fetches the first "page" of the collection. See [pagination](/docs/pagination) for more detail.<br/>
* `token` - _optional_ - Authentication token. Requires scope: `none`<br/>
* `limit` - _optional_ - The maximum number of items to return.<br/>

### apps_permissions_users_request
> Enables an app to trigger a permissions modal to grant an app access to a user access scope.<br/>

*Tags:* `apps.permissions.users` `apps`

#### Input Parameters
* `scopes` - _optional_ - A comma separated list of user scopes to request for<br/>
* `token` - _optional_ - Authentication token. Requires scope: `none`<br/>
* `user` - _optional_ - The user this scope is being requested for<br/>
* `trigger_id` - _optional_ - Token used to trigger the request<br/>

### apps_uninstall
> Uninstalls your app from a workspace.<br/>

*Tags:* `apps`

#### Input Parameters
* `client_secret` - _optional_ - Issued when you created your application.<br/>
* `token` - _optional_ - Authentication token. Requires scope: `none`<br/>
* `client_id` - _optional_ - Issued when you created your application.<br/>

### auth_revoke
> Revokes a token.<br/>

*Tags:* `auth`

#### Input Parameters
* `test` - _optional_ - Setting this parameter to `1` triggers a _testing mode_ where the specified token will not actually be revoked.<br/>
* `token` - _optional_ - Authentication token. Requires scope: `none`<br/>

### auth_test
> Checks authentication & identity.<br/>

*Tags:* `auth`

### bots_info
> Gets information about a bot user.<br/>

*Tags:* `bots`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `users:read`<br/>
* `bot` - _optional_ - Bot user to get info on<br/>

### channels_archive
> Archives a channel.<br/>

*Tags:* `channels`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `channels:write`<br/>

### channels_create
> Creates a channel.<br/>

*Tags:* `channels`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `channels:write`<br/>

### channels_history
> Fetches history of messages and events from a channel.<br/>

*Tags:* `channels`

#### Input Parameters
* `count` - _optional_ - Number of messages to return, between 1 and 1000.<br/>
* `unreads` - _optional_ - Include `unread_count_display` in the output?<br/>
* `inclusive` - _optional_ - Include messages with latest or oldest timestamp in results.<br/>
* `token` - _optional_ - Authentication token. Requires scope: `channels:history`<br/>
* `oldest` - _optional_ - Start of time range of messages to include in results.<br/>
* `channel` - _optional_ - Channel to fetch history for.<br/>
* `latest` - _optional_ - End of time range of messages to include in results.<br/>

### channels_info
> Gets information about a channel.<br/>

*Tags:* `channels`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `channels:read`<br/>
* `include_locale` - _optional_ - Set this to `true` to receive the locale for this channel. Defaults to `false`<br/>
* `channel` - _optional_ - Channel to get info on<br/>

### channels_invite
> Invites a user to a channel.<br/>

*Tags:* `channels`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `channels:write`<br/>

### channels_join
> Joins a channel, creating it if needed.<br/>

*Tags:* `channels`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `channels:write`<br/>

### channels_kick
> Removes a user from a channel.<br/>

*Tags:* `channels`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `channels:write`<br/>

### channels_leave
> Leaves a channel.<br/>

*Tags:* `channels`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `channels:write`<br/>

### channels_list
> Lists all channels in a Slack team.<br/>

*Tags:* `channels`

#### Input Parameters
* `exclude_members` - _optional_ - Exclude the `members` collection from each `channel`<br/>
* `cursor` - _optional_ - Paginate through collections of data by setting the `cursor` parameter to a `next_cursor` attribute returned by a previous request's `response_metadata`. Default value fetches the first "page" of the collection. See [pagination](/docs/pagination) for more detail.<br/>
* `token` - _optional_ - Authentication token. Requires scope: `channels:read`<br/>
* `limit` - _optional_ - The maximum number of items to return. Fewer than the requested number of items may be returned, even if the end of the users list hasn't been reached.<br/>
* `exclude_archived` - _optional_ - Exclude archived channels from the list<br/>

### channels_mark
> Sets the read cursor in a channel.<br/>

*Tags:* `channels`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `channels:write`<br/>

### channels_rename
> Renames a channel.<br/>

*Tags:* `channels`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `channels:write`<br/>

### channels_replies
> Retrieve a thread of messages posted to a channel<br/>

*Tags:* `channels`

#### Input Parameters
* `thread_ts` - _optional_ - Unique identifier of a thread's parent message<br/>
* `token` - _optional_ - Authentication token. Requires scope: `channels:history`<br/>
* `channel` - _optional_ - Channel to fetch thread from<br/>

### channels_setPurpose
> Sets the purpose for a channel.<br/>

*Tags:* `channels`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `channels:write`<br/>

### channels_setTopic
> Sets the topic for a channel.<br/>

*Tags:* `channels`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `channels:write`<br/>

### channels_unarchive
> Unarchives a channel.<br/>

*Tags:* `channels`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `channels:write`<br/>

### chat_delete
> Deletes a message.<br/>

*Tags:* `chat`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `chat:write`<br/>

### chat_deleteScheduledMessage
> Deletes a pending scheduled message from the queue.<br/>

*Tags:* `chat`

### chat_getPermalink
> Retrieve a permalink URL for a specific extant message<br/>

*Tags:* `chat`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `none`<br/>
* `message_ts` - _optional_ - A message's `ts` value, uniquely identifying it within a channel<br/>
* `channel` - _optional_ - The ID of the conversation or channel containing the message<br/>

### chat_meMessage
> Share a me message into a channel.<br/>

*Tags:* `chat`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `chat:write:user`<br/>

### chat_postEphemeral
> Sends an ephemeral message to a user in a channel.<br/>

*Tags:* `chat`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `chat:write`<br/>

### chat_postMessage
> Sends a message to a channel.<br/>

*Tags:* `chat`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `chat:write`<br/>

### chat_scheduleMessage
> Schedules a message to be sent to a channel.<br/>

*Tags:* `chat`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `chat:write`<br/>

### chat_scheduledMessages_list
> Returns a list of scheduled messages.<br/>

*Tags:* `chat.scheduledMessages` `chat`

#### Input Parameters
* `cursor` - _optional_ - For pagination purposes, this is the `cursor` value returned from a previous call to `chat.scheduledmessages.list` indicating where you want to start this call from.<br/>
* `token` - _optional_ - Authentication token. Requires scope: `none`<br/>
* `limit` - _optional_ - Maximum number of original entries to return.<br/>
* `oldest` - _optional_ - A UNIX timestamp of the oldest value in the time range<br/>
* `channel` - _optional_ - The channel of the scheduled messages<br/>
* `latest` - _optional_ - A UNIX timestamp of the latest value in the time range<br/>

### chat_unfurl
> Provide custom unfurl behavior for user-posted URLs<br/>

*Tags:* `chat`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `links:write`<br/>

### chat_update
> Updates a message.<br/>

*Tags:* `chat`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `chat:write`<br/>

### conversations_archive
> Archives a conversation.<br/>

*Tags:* `conversations`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `conversations:write`<br/>

### conversations_close
> Closes a direct message or multi-person direct message.<br/>

*Tags:* `conversations`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `conversations:write`<br/>

### conversations_create
> Initiates a public or private channel-based conversation<br/>

*Tags:* `conversations`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `conversations:write`<br/>

### conversations_history
> Fetches a conversation's history of messages and events.<br/>

*Tags:* `conversations`

#### Input Parameters
* `inclusive` - _optional_ - Include messages with latest or oldest timestamp in results only when either timestamp is specified.<br/>
* `cursor` - _optional_ - Paginate through collections of data by setting the `cursor` parameter to a `next_cursor` attribute returned by a previous request's `response_metadata`. Default value fetches the first "page" of the collection. See [pagination](/docs/pagination) for more detail.<br/>
* `token` - _optional_ - Authentication token. Requires scope: `conversations:history`<br/>
* `limit` - _optional_ - The maximum number of items to return. Fewer than the requested number of items may be returned, even if the end of the users list hasn't been reached.<br/>
* `oldest` - _optional_ - Start of time range of messages to include in results.<br/>
* `channel` - _optional_ - Conversation ID to fetch history for.<br/>
* `latest` - _optional_ - End of time range of messages to include in results.<br/>

### conversations_info
> Retrieve information about a conversation.<br/>

*Tags:* `conversations`

#### Input Parameters
* `include_num_members` - _optional_ - Set to `true` to include the member count for the specified conversation. Defaults to `false`<br/>
* `token` - _optional_ - Authentication token. Requires scope: `conversations:read`<br/>
* `channel` - _optional_ - Conversation ID to learn more about<br/>
* `include_locale` - _optional_ - Set this to `true` to receive the locale for this conversation. Defaults to `false`<br/>

### conversations_invite
> Invites users to a channel.<br/>

*Tags:* `conversations`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `conversations:write`<br/>

### conversations_join
> Joins an existing conversation.<br/>

*Tags:* `conversations`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `channels:write`<br/>

### conversations_kick
> Removes a user from a conversation.<br/>

*Tags:* `conversations`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `conversations:write`<br/>

### conversations_leave
> Leaves a conversation.<br/>

*Tags:* `conversations`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `conversations:write`<br/>

### conversations_list
> Lists all channels in a Slack team.<br/>

*Tags:* `conversations`

#### Input Parameters
* `cursor` - _optional_ - Paginate through collections of data by setting the `cursor` parameter to a `next_cursor` attribute returned by a previous request's `response_metadata`. Default value fetches the first "page" of the collection. See [pagination](/docs/pagination) for more detail.<br/>
* `token` - _optional_ - Authentication token. Requires scope: `conversations:read`<br/>
* `limit` - _optional_ - The maximum number of items to return. Fewer than the requested number of items may be returned, even if the end of the list hasn't been reached. Must be an integer no larger than 1000.<br/>
* `exclude_archived` - _optional_ - Set to `true` to exclude archived channels from the list<br/>
* `types` - _optional_ - Mix and match channel types by providing a comma-separated list of any combination of `public_channel`, `private_channel`, `mpim`, `im`<br/>

### conversations_members
> Retrieve members of a conversation.<br/>

*Tags:* `conversations`

#### Input Parameters
* `cursor` - _optional_ - Paginate through collections of data by setting the `cursor` parameter to a `next_cursor` attribute returned by a previous request's `response_metadata`. Default value fetches the first "page" of the collection. See [pagination](/docs/pagination) for more detail.<br/>
* `token` - _optional_ - Authentication token. Requires scope: `conversations:read`<br/>
* `limit` - _optional_ - The maximum number of items to return. Fewer than the requested number of items may be returned, even if the end of the users list hasn't been reached.<br/>
* `channel` - _optional_ - ID of the conversation to retrieve members for<br/>

### conversations_open
> Opens or resumes a direct message or multi-person direct message.<br/>

*Tags:* `conversations`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `conversations:write`<br/>

### conversations_rename
> Renames a conversation.<br/>

*Tags:* `conversations`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `conversations:write`<br/>

### conversations_replies
> Retrieve a thread of messages posted to a conversation<br/>

*Tags:* `conversations`

#### Input Parameters
* `inclusive` - _optional_ - Include messages with latest or oldest timestamp in results only when either timestamp is specified.<br/>
* `ts` - _optional_ - Unique identifier of a thread's parent message.<br/>
* `cursor` - _optional_ - Paginate through collections of data by setting the `cursor` parameter to a `next_cursor` attribute returned by a previous request's `response_metadata`. Default value fetches the first "page" of the collection. See [pagination](/docs/pagination) for more detail.<br/>
* `token` - _optional_ - Authentication token. Requires scope: `conversations:history`<br/>
* `limit` - _optional_ - The maximum number of items to return. Fewer than the requested number of items may be returned, even if the end of the users list hasn't been reached.<br/>
* `oldest` - _optional_ - Start of time range of messages to include in results.<br/>
* `channel` - _optional_ - Conversation ID to fetch thread from.<br/>
* `latest` - _optional_ - End of time range of messages to include in results.<br/>

### conversations_setPurpose
> Sets the purpose for a conversation.<br/>

*Tags:* `conversations`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `conversations:write`<br/>

### conversations_setTopic
> Sets the topic for a conversation.<br/>

*Tags:* `conversations`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `conversations:write`<br/>

### conversations_unarchive
> Reverses conversation archival.<br/>

*Tags:* `conversations`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `conversations:write`<br/>

### dialog_open
> Open a dialog with a user<br/>

*Tags:* `dialog`

### dnd_endDnd
> Ends the current user's Do Not Disturb session immediately.<br/>

*Tags:* `dnd`

### dnd_endSnooze
> Ends the current user's snooze mode immediately.<br/>

*Tags:* `dnd`

### dnd_info
> Retrieves a user's current Do Not Disturb status.<br/>

*Tags:* `dnd`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `dnd:read`<br/>
* `user` - _optional_ - User to fetch status for (defaults to current user)<br/>

### dnd_setSnooze
> Turns on Do Not Disturb mode for the current user, or changes its duration.<br/>

*Tags:* `dnd`

### dnd_teamInfo
> Retrieves the Do Not Disturb status for up to 50 users on a team.<br/>

*Tags:* `dnd`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `dnd:read`<br/>
* `users` - _optional_ - Comma-separated list of users to fetch Do Not Disturb status for<br/>

### emoji_list
> Lists custom emoji for a team.<br/>

*Tags:* `emoji`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `emoji:read`<br/>

### files_comments_delete
> Deletes an existing comment on a file.<br/>

*Tags:* `files.comments` `files`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `files:write:user`<br/>

### files_delete
> Deletes a file.<br/>

*Tags:* `files`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `files:write:user`<br/>

### files_info
> Gets information about a team file.<br/>

*Tags:* `files`

#### Input Parameters
* `count` - _optional_
* `cursor` - _optional_ - Parameter for pagination. File comments are paginated for a single file. Set `cursor` equal to the `next_cursor` attribute returned by the previous request's `response_metadata`. This parameter is optional, but pagination is mandatory: the default value simply fetches the first "page" of the collection of comments. See [pagination](/docs/pagination) for more details.<br/>
* `token` - _optional_ - Authentication token. Requires scope: `files:read`<br/>
* `limit` - _optional_ - The maximum number of items to return. Fewer than the requested number of items may be returned, even if the end of the list hasn't been reached.<br/>
* `file` - _optional_ - Specify a file by providing its ID.<br/>
* `page` - _optional_

### files_list
> Lists & filters team files.<br/>

*Tags:* `files`

#### Input Parameters
* `count` - _optional_
* `channel` - _optional_ - Filter files appearing in a specific channel, indicated by its ID.<br/>
* `ts_to` - _optional_ - Filter files created before this timestamp (inclusive).<br/>
* `ts_from` - _optional_ - Filter files created after this timestamp (inclusive).<br/>
* `token` - _optional_ - Authentication token. Requires scope: `files:read`<br/>
* `user` - _optional_ - Filter files created by a single user.<br/>
* `page` - _optional_
* `types` - _optional_ - Filter files by type ([see below](#file_types)). You can pass multiple values in the types argument, like `types=spaces,snippets`.The default value is `all`, which does not filter the list.<br/>

### files_revokePublicURL
> Revokes public/external sharing access for a file<br/>

*Tags:* `files`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `files:write:user`<br/>

### files_sharedPublicURL
> Enables a file for public/external sharing.<br/>

*Tags:* `files`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `files:write:user`<br/>

### files_upload
> Uploads or creates a file.<br/>

*Tags:* `files`

### groups_archive
> Archives a private channel.<br/>

*Tags:* `groups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `groups:write`<br/>

### groups_create
> Creates a private channel.<br/>

*Tags:* `groups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `groups:write`<br/>

### groups_createChild
> Clones and archives a private channel.<br/>

*Tags:* `groups`

### groups_history
> Fetches history of messages and events from a private channel.<br/>

*Tags:* `groups`

#### Input Parameters
* `count` - _optional_ - Number of messages to return, between 1 and 1000.<br/>
* `unreads` - _optional_ - Include `unread_count_display` in the output?<br/>
* `inclusive` - _optional_ - Include messages with latest or oldest timestamp in results.<br/>
* `token` - _optional_ - Authentication token. Requires scope: `groups:history`<br/>
* `oldest` - _optional_ - Start of time range of messages to include in results.<br/>
* `channel` - _optional_ - Private channel to fetch history for.<br/>
* `latest` - _optional_ - End of time range of messages to include in results.<br/>

### groups_info
> Gets information about a private channel.<br/>

*Tags:* `groups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `groups:read`<br/>
* `include_locale` - _optional_ - Set this to `true` to receive the locale for this group. Defaults to `false`<br/>
* `channel` - _optional_ - Private channel to get info on<br/>

### groups_invite
> Invites a user to a private channel.<br/>

*Tags:* `groups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `groups:write`<br/>

### groups_kick
> Removes a user from a private channel.<br/>

*Tags:* `groups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `groups:write`<br/>

### groups_leave
> Leaves a private channel.<br/>

*Tags:* `groups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `groups:write`<br/>

### groups_list
> Lists private channels that the calling user has access to.<br/>

*Tags:* `groups`

#### Input Parameters
* `cursor` - _optional_ - Parameter for pagination. Set `cursor` equal to the `next_cursor` attribute returned by the previous request's `response_metadata`. This parameter is optional, but pagination is mandatory: the default value simply fetches the first "page" of the collection. See [pagination](/docs/pagination) for more details.<br/>
* `exclude_members` - _optional_ - Exclude the `members` from each `group`<br/>
* `token` - _optional_ - Authentication token. Requires scope: `groups:read`<br/>
* `exclude_archived` - _optional_ - Don't return archived private channels.<br/>
* `limit` - _optional_ - The maximum number of items to return. Fewer than the requested number of items may be returned, even if the end of the list hasn't been reached.<br/>

### groups_mark
> Sets the read cursor in a private channel.<br/>

*Tags:* `groups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `groups:write`<br/>

### groups_open
> Opens a private channel.<br/>

*Tags:* `groups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `groups:write`<br/>

### groups_rename
> Renames a private channel.<br/>

*Tags:* `groups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `groups:write`<br/>

### groups_replies
> Retrieve a thread of messages posted to a private channel<br/>

*Tags:* `groups`

#### Input Parameters
* `thread_ts` - _optional_ - Unique identifier of a thread's parent message<br/>
* `token` - _optional_ - Authentication token. Requires scope: `groups:history`<br/>
* `channel` - _optional_ - Private channel to fetch thread from<br/>

### groups_setPurpose
> Sets the purpose for a private channel.<br/>

*Tags:* `groups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `groups:write`<br/>

### groups_setTopic
> Sets the topic for a private channel.<br/>

*Tags:* `groups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `groups:write`<br/>

### groups_unarchive
> Unarchives a private channel.<br/>

*Tags:* `groups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `groups:write`<br/>

### im_close
> Close a direct message channel.<br/>

*Tags:* `im`

### im_history
> Fetches history of messages and events from direct message channel.<br/>

*Tags:* `im`

#### Input Parameters
* `count` - _optional_ - Number of messages to return, between 1 and 1000.<br/>
* `unreads` - _optional_ - Include `unread_count_display` in the output?<br/>
* `inclusive` - _optional_ - Include messages with latest or oldest timestamp in results.<br/>
* `token` - _optional_ - Authentication token. Requires scope: `im:history`<br/>
* `oldest` - _optional_ - Start of time range of messages to include in results.<br/>
* `channel` - _optional_ - Direct message channel to fetch history for.<br/>
* `latest` - _optional_ - End of time range of messages to include in results.<br/>

### im_list
> Lists direct message channels for the calling user.<br/>

*Tags:* `im`

#### Input Parameters
* `cursor` - _optional_ - Paginate through collections of data by setting the `cursor` parameter to a `next_cursor` attribute returned by a previous request's `response_metadata`. Default value fetches the first "page" of the collection. See [pagination](/docs/pagination) for more detail.<br/>
* `token` - _optional_ - Authentication token. Requires scope: `im:read`<br/>
* `limit` - _optional_ - The maximum number of items to return. Fewer than the requested number of items may be returned, even if the end of the users list hasn't been reached.<br/>

### im_mark
> Sets the read cursor in a direct message channel.<br/>

*Tags:* `im`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `im:write`<br/>

### im_open
> Opens a direct message channel.<br/>

*Tags:* `im`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `im:write`<br/>

### im_replies
> Retrieve a thread of messages posted to a direct message conversation<br/>

*Tags:* `im`

#### Input Parameters
* `thread_ts` - _optional_ - Unique identifier of a thread's parent message<br/>
* `token` - _optional_ - Authentication token. Requires scope: `im:history`<br/>
* `channel` - _optional_ - Direct message channel to fetch thread from<br/>

### migration_exchange
> For Enterprise Grid workspaces, map local user IDs to global user IDs<br/>

*Tags:* `migration`

### mpim_close
> Closes a multiparty direct message channel.<br/>

*Tags:* `mpim`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `mpim:write`<br/>

### mpim_history
> Fetches history of messages and events from a multiparty direct message.<br/>

*Tags:* `mpim`

#### Input Parameters
* `count` - _optional_ - Number of messages to return, between 1 and 1000.<br/>
* `unreads` - _optional_ - Include `unread_count_display` in the output?<br/>
* `inclusive` - _optional_ - Include messages with latest or oldest timestamp in results.<br/>
* `token` - _optional_ - Authentication token. Requires scope: `mpim:history`<br/>
* `oldest` - _optional_ - Start of time range of messages to include in results.<br/>
* `channel` - _optional_ - Multiparty direct message to fetch history for.<br/>
* `latest` - _optional_ - End of time range of messages to include in results.<br/>

### mpim_list
> Lists multiparty direct message channels for the calling user.<br/>

*Tags:* `mpim`

#### Input Parameters
* `cursor` - _optional_ - Parameter for pagination. Set `cursor` equal to the `next_cursor` attribute returned by the previous request's `response_metadata`. This parameter is optional, but pagination is mandatory: the default value simply fetches the first "page" of the collection. See [pagination](/docs/pagination) for more details.<br/>
* `token` - _optional_ - Authentication token. Requires scope: `mpim:read`<br/>
* `limit` - _optional_ - The maximum number of items to return. Fewer than the requested number of items may be returned, even if the end of the list hasn't been reached.<br/>

### mpim_mark
> Sets the read cursor in a multiparty direct message channel.<br/>

*Tags:* `mpim`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `mpim:write`<br/>

### mpim_open
> This method opens a multiparty direct message.<br/>

*Tags:* `mpim`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `mpim:write`<br/>

### mpim_replies
> Retrieve a thread of messages posted to a direct message conversation from a multiparty direct message.<br/>

*Tags:* `mpim`

#### Input Parameters
* `thread_ts` - _optional_ - Unique identifier of a thread's parent message.<br/>
* `token` - _optional_ - Authentication token. Requires scope: `mpim:history`<br/>
* `channel` - _optional_ - Multiparty direct message channel to fetch thread from.<br/>

### oauth_access
> Exchanges a temporary OAuth verifier code for an access token.<br/>

*Tags:* `oauth`

#### Input Parameters
* `code` - _optional_ - The `code` param returned via the OAuth callback.<br/>
* `redirect_uri` - _optional_ - This must match the originally submitted URI (if one was sent).<br/>
* `client_id` - _optional_ - Issued when you created your application.<br/>
* `client_secret` - _optional_ - Issued when you created your application.<br/>
* `single_channel` - _optional_ - Request the user to add your app only to a single channel.<br/>

### oauth_token
> Exchanges a temporary OAuth verifier code for a workspace token.<br/>

*Tags:* `oauth`

#### Input Parameters
* `client_secret` - _optional_ - Issued when you created your application.<br/>
* `code` - _optional_ - The `code` param returned via the OAuth callback.<br/>
* `single_channel` - _optional_ - Request the user to add your app only to a single channel.<br/>
* `client_id` - _optional_ - Issued when you created your application.<br/>
* `redirect_uri` - _optional_ - This must match the originally submitted URI (if one was sent).<br/>

### pins_add
> Pins an item to a channel.<br/>

*Tags:* `pins`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `pins:write`<br/>

### pins_list
> Lists items pinned to a channel.<br/>

*Tags:* `pins`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `pins:read`<br/>
* `channel` - _optional_ - Channel to get pinned items for.<br/>

### pins_remove
> Un-pins an item from a channel.<br/>

*Tags:* `pins`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `pins:write`<br/>

### reactions_add
> Adds a reaction to an item.<br/>

*Tags:* `reactions`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `reactions:write`<br/>

### reactions_get
> Gets reactions for an item.<br/>

*Tags:* `reactions`

#### Input Parameters
* `full` - _optional_ - If true always return the complete reaction list.<br/>
* `file_comment` - _optional_ - File comment to get reactions for.<br/>
* `timestamp` - _optional_ - Timestamp of the message to get reactions for.<br/>
* `token` - _optional_ - Authentication token. Requires scope: `reactions:read`<br/>
* `file` - _optional_ - File to get reactions for.<br/>
* `channel` - _optional_ - Channel where the message to get reactions for was posted.<br/>

### reactions_list
> Lists reactions made by a user.<br/>

*Tags:* `reactions`

#### Input Parameters
* `count` - _optional_
* `full` - _optional_ - If true always return the complete reaction list.<br/>
* `cursor` - _optional_ - Parameter for pagination. Set `cursor` equal to the `next_cursor` attribute returned by the previous request's `response_metadata`. This parameter is optional, but pagination is mandatory: the default value simply fetches the first "page" of the collection. See [pagination](/docs/pagination) for more details.<br/>
* `token` - _optional_ - Authentication token. Requires scope: `reactions:read`<br/>
* `limit` - _optional_ - The maximum number of items to return. Fewer than the requested number of items may be returned, even if the end of the list hasn't been reached.<br/>
* `user` - _optional_ - Show reactions made by this user. Defaults to the authed user.<br/>
* `page` - _optional_

### reactions_remove
> Removes a reaction from an item.<br/>

*Tags:* `reactions`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `reactions:write`<br/>

### reminders_add
> Creates a reminder.<br/>

*Tags:* `reminders`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `reminders:write`<br/>

### reminders_complete
> Marks a reminder as complete.<br/>

*Tags:* `reminders`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `reminders:write`<br/>

### reminders_delete
> Deletes a reminder.<br/>

*Tags:* `reminders`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `reminders:write`<br/>

### reminders_info
> Gets information about a reminder.<br/>

*Tags:* `reminders`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `reminders:read`<br/>
* `reminder` - _optional_ - The ID of the reminder<br/>

### reminders_list
> Lists all reminders created by or for a given user.<br/>

*Tags:* `reminders`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `reminders:read`<br/>

### rtm_connect
> Starts a Real Time Messaging session.<br/>

*Tags:* `rtm`

#### Input Parameters
* `presence_sub` - _optional_ - Only deliver presence events when requested by subscription. See [presence subscriptions](/docs/presence-and-status#subscriptions).<br/>
* `token` - _optional_ - Authentication token. Requires scope: `rtm:stream`<br/>
* `batch_presence_aware` - _optional_ - Batch presence deliveries via subscription. Enabling changes the shape of `presence_change` events. See [batch presence](/docs/presence-and-status#batching).<br/>

### search_messages
> Searches for messages matching a query.<br/>

*Tags:* `search`

#### Input Parameters
* `sort_dir` - _optional_ - Change sort direction to ascending (`asc`) or descending (`desc`).<br/>
* `query` - _optional_ - Search query.<br/>
* `sort` - _optional_ - Return matches sorted by either `score` or `timestamp`.<br/>
* `count` - _optional_ - Pass the number of results you want per "page". Maximum of `100`.<br/>
* `token` - _optional_ - Authentication token. Requires scope: `search:read`<br/>
* `highlight` - _optional_ - Pass a value of `true` to enable query highlight markers (see below).<br/>
* `page` - _optional_

### stars_add
> Adds a star to an item.<br/>

*Tags:* `stars`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `stars:write`<br/>

### stars_list
> Lists stars for a user.<br/>

*Tags:* `stars`

#### Input Parameters
* `count` - _optional_
* `cursor` - _optional_ - Parameter for pagination. Set `cursor` equal to the `next_cursor` attribute returned by the previous request's `response_metadata`. This parameter is optional, but pagination is mandatory: the default value simply fetches the first "page" of the collection. See [pagination](/docs/pagination) for more details.<br/>
* `token` - _optional_ - Authentication token. Requires scope: `stars:read`<br/>
* `limit` - _optional_ - The maximum number of items to return. Fewer than the requested number of items may be returned, even if the end of the list hasn't been reached.<br/>
* `page` - _optional_

### stars_remove
> Removes a star from an item.<br/>

*Tags:* `stars`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `stars:write`<br/>

### team_accessLogs
> Gets the access logs for the current team.<br/>

*Tags:* `team`

#### Input Parameters
* `count` - _optional_
* `token` - _optional_ - Authentication token. Requires scope: `admin`<br/>
* `page` - _optional_
* `before` - _optional_ - End of time range of logs to include in results (inclusive).<br/>

### team_billableInfo
> Gets billable users information for the current team.<br/>

*Tags:* `team`

### team_info
> Gets information about the current team.<br/>

*Tags:* `team`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `team:read`<br/>
* `team` - _optional_ - Team to get info on, if omitted, will return information about the current team. Will only return team that the authenticated token is allowed to see through external shared channels<br/>

### team_integrationLogs
> Gets the integration logs for the current team.<br/>

*Tags:* `team`

#### Input Parameters
* `count` - _optional_
* `change_type` - _optional_ - Filter logs with this change type. Defaults to all logs.<br/>
* `app_id` - _optional_ - Filter logs to this Slack app. Defaults to all logs.<br/>
* `token` - _optional_ - Authentication token. Requires scope: `admin`<br/>
* `user` - _optional_ - Filter logs generated by this user's actions. Defaults to all logs.<br/>
* `service_id` - _optional_ - Filter logs to this service. Defaults to all logs.<br/>
* `page` - _optional_

### team_profile_get
> Retrieve a team's profile.<br/>

*Tags:* `team.profile` `team`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `users.profile:read`<br/>
* `visibility` - _optional_ - Filter by visibility.<br/>

### usergroups_create
> Create a User Group<br/>

*Tags:* `usergroups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `usergroups:write`<br/>

### usergroups_disable
> Disable an existing User Group<br/>

*Tags:* `usergroups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `usergroups:write`<br/>

### usergroups_enable
> Enable a User Group<br/>

*Tags:* `usergroups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `usergroups:write`<br/>

### usergroups_list
> List all User Groups for a team<br/>

*Tags:* `usergroups`

#### Input Parameters
* `include_users` - _optional_ - Include the list of users for each User Group.<br/>
* `token` - _optional_ - Authentication token. Requires scope: `usergroups:read`<br/>
* `include_count` - _optional_ - Include the number of users in each User Group.<br/>
* `include_disabled` - _optional_ - Include disabled User Groups.<br/>

### usergroups_update
> Update an existing User Group<br/>

*Tags:* `usergroups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `usergroups:write`<br/>

### usergroups_users_list
> List all users in a User Group<br/>

*Tags:* `usergroups.users` `usergroups`

### usergroups_users_update
> Update the list of users for a User Group<br/>

*Tags:* `usergroups.users` `usergroups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `usergroups:write`<br/>

### users_conversations
> List conversations the calling user may access.<br/>

*Tags:* `users`

#### Input Parameters
* `cursor` - _optional_ - Paginate through collections of data by setting the `cursor` parameter to a `next_cursor` attribute returned by a previous request's `response_metadata`. Default value fetches the first "page" of the collection. See [pagination](/docs/pagination) for more detail.<br/>
* `token` - _optional_ - Authentication token. Requires scope: `conversations:read`<br/>
* `limit` - _optional_ - The maximum number of items to return. Fewer than the requested number of items may be returned, even if the end of the list hasn't been reached. Must be an integer no larger than 1000.<br/>
* `user` - _optional_ - Browse conversations by a specific user ID's membership. Non-public channels are restricted to those where the calling user shares membership.<br/>
* `exclude_archived` - _optional_ - Set to `true` to exclude archived channels from the list<br/>
* `types` - _optional_ - Mix and match channel types by providing a comma-separated list of any combination of `public_channel`, `private_channel`, `mpim`, `im`<br/>

### users_deletePhoto
> Delete the user profile photo<br/>

*Tags:* `users`

### users_getPresence
> Gets user presence information.<br/>

*Tags:* `users`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `users:read`<br/>
* `user` - _optional_ - User to get presence info on. Defaults to the authed user.<br/>

### users_identity
> Get a user's identity.<br/>

*Tags:* `users`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `identity.basic`<br/>

### users_info
> Gets information about a user.<br/>

*Tags:* `users`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `users:read`<br/>
* `user` - _optional_ - User to get info on<br/>
* `include_locale` - _optional_ - Set this to `true` to receive the locale for this user. Defaults to `false`<br/>

### users_list
> Lists all users in a Slack team.<br/>

*Tags:* `users`

#### Input Parameters
* `cursor` - _optional_ - Paginate through collections of data by setting the `cursor` parameter to a `next_cursor` attribute returned by a previous request's `response_metadata`. Default value fetches the first "page" of the collection. See [pagination](/docs/pagination) for more detail.<br/>
* `token` - _optional_ - Authentication token. Requires scope: `users:read`<br/>
* `limit` - _optional_ - The maximum number of items to return. Fewer than the requested number of items may be returned, even if the end of the users list hasn't been reached.<br/>
* `include_locale` - _optional_ - Set this to `true` to receive the locale for users. Defaults to `false`<br/>

### users_lookupByEmail
> Find a user with an email address.<br/>

*Tags:* `users`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `users:read.email`<br/>
* `email` - _optional_ - An email address belonging to a user in the workspace<br/>

### users_profile_get
> Retrieves a user's profile information.<br/>

*Tags:* `users.profile` `users`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `users.profile:read`<br/>
* `include_labels` - _optional_ - Include labels for each ID in custom profile fields<br/>
* `user` - _optional_ - User to retrieve profile info for<br/>

### users_profile_set
> Set the profile information for a user.<br/>

*Tags:* `users.profile` `users`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `users.profile:write`<br/>

### users_setActive
> Marked a user as active. Deprecated and non-functional.<br/>

*Tags:* `users`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `users:write`<br/>

### users_setPhoto
> Set the user profile photo<br/>

*Tags:* `users`

### users_setPresence
> Manually sets user presence.<br/>

*Tags:* `users`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `users:write`<br/>

## License

**flow**ground :- Telekom iPaaS / slack-web-api-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
