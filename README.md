# getdrip-api
A nodejs wrapper for drip  v2 api.

#### Usage
    var getdrip = require('getdripapi')(apiToken, accountId);
    
# Supported APIs

## [Accounts](https://www.getdrip.com/docs/rest-api#accounts)

### `.getAccounts` 
returns a list of accounts
#### Usage
    getdrip.getAccounts(function(err, res, body){
       // body contains account list
    }

## [Subscribers](https://www.getdrip.com/docs/rest-api#subscribers)

### `.getSubscribers` 
 returns list of subscribers
#### Usage
    getdrip.getSubscribers = function (cb) {
        // returns list of subscribers
    }
    
### `.getSubscriber` 
returns a single subscriber
#### Usage
    getdrip.getSubscriber = function (subscriberId, function(err, res, body) {
        // returns list of one subscriber
    })
    
### `.createSubscriber`
returns a subscriber
#### Usage
    getdrip.createSubscriber(testEmail, {}, function(err, res, body) {
        // returns list of the new subscriber
    })

## [Campaigns](https://www.getdrip.com/docs/rest-api#campaigns)

### `.getCampaigns` 
returns list of campgains
#### Usage
    getdrip.getCampaigns = function (cb) {
        // returns list of subscribers
    }
    
### `.subscribeToCampaign` 
adds a subscriber to a campaign
#### Usage
    getdrip.subscribeToCampaign(email, campaignId, {}, function(err, res, body) {
        // returns list of subscribers added to the campaign
    }
    
    

## [Events](https://www.getdrip.com/docs/rest-api#events)

### `.createEvent` 
creates an event for a given subscriber
#### Usage
    getdrip.createEvent = function (email, event, opts, function(err, res, body) {
        // no body
    }
    
## [Tags](https://www.getdrip.com/docs/rest-api#tags)

### `.createTag` 
creates a tag for a given subscriber
#### Usage
    getdrip.createEvent = function (email, tag, opts, function(err, res, body) {
        // no body
    }

# License
[MIT](https://github.com/eatrero/getdrip-api/blob/master/MIT-LICENSE.txt)