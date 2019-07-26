# ![LOGO](logo.png) groupalarm Pager API **flow**ground Connector

## Description

A generated **flow**ground connector for the groupalarm Pager API API (version 1.15.0).

Generated from: https://app.groupalarm.com/api/v1/pager<br/>
Generated at: 2019-07-26T13:59:35+03:00

## API Description

The pager service implements all pager functions for GroupAlarm<br/>
<br/>
# Authentication<br/>
<br/>
<!-- ReDoc-Inject: <security-definitions> --><br/>

## Authorization

Supported authorization schemes:
- API Key
- API Key

## Actions

### ListPager
> Returns all pagers for current user or given organization<br/>

*Tags:* `pager`

#### Input Parameters
* `owner_id` - _optional_ - requested user<br/>
* `organization_id` - _optional_ - requested organization<br/>

### CreatePager
> Create a pager configuration in the given organization<br/>

*Tags:* `pager`

### GetPager
> Returns all information about the pager and the current status data<br/>

*Tags:* `pager`

#### Input Parameters
* `pagerID` - _required_ - ID of an existing pager<br/>
* `organization_id` - _required_ - requesting organization<br/>

### UpdatePager
> Updates an existing pager configuration<br/>

*Tags:* `pager`

#### Input Parameters
* `pagerID` - _required_ - ID of an existing pager configuration<br/>

### RemovePagerFromOrganization
> Remove a pager from the given organization<br/>

*Tags:* `pager`

#### Input Parameters
* `pagerID` - _required_ - ID of an existing pager configuration<br/>
* `organization_id` - _required_ - requested organization<br/>

### AssignPagerToUser
> Set a pager as personal device of the given user<br/>

*Tags:* `pager`

#### Input Parameters
* `pagerID` - _required_ - ID of an existing pager configuration<br/>
* `userID` - _required_ - ID of an existing user<br/>
* `organization_id` - _optional_ - requesting organization; zero if user<br/>

### GetDisabledOrganization
> Returns whether the given organization has disabled this way of alarming or not<br/>

*Tags:* `organizations`

#### Input Parameters
* `organization_id` - _required_ - requesting organization<br/>

### SetDisabledOrganization
> Sets whether the given organization has this way of alarming disabled or not<br/>

*Tags:* `organizations`

#### Input Parameters
* `organization_id` - _required_ - requesting organization<br/>

### Init
> Force a pager to init itself again<br/>

*Tags:* `management`

### Lock
> Lock the pager and prevent any further use<br/>

*Tags:* `management`

### Reset
> Force a pager to reset (to default settings)<br/>

*Tags:* `management`

### Status
> Request a status update from the pager<br/>

*Tags:* `management`

### Alarm
> Send the given text like an alarm onto the pager's display<br/>

*Tags:* `management`

### Display
> Display the given text on the pager's display<br/>

*Tags:* `management`

### Unlock
> Unlock the pager and allow usage<br/>

*Tags:* `management`

### Update
> Force a pager to run an update<br/>

*Tags:* `management`

### Statistics
> Returns pager statistics for given organization<br/>

*Tags:* `pager`

#### Input Parameters
* `organization_id` - _required_ - requested organization<br/>

## License

**flow**ground :- Telekom iPaaS / groupalarm-pager-api-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
