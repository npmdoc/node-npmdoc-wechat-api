# api documentation for  [wechat-api (v1.32.0)](https://github.com/node-webot/wechat-api#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-wechat-api.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-wechat-api) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-wechat-api.svg)](https://travis-ci.org/npmdoc/node-npmdoc-wechat-api)
#### 微信公共平台Node库 API

[![NPM](https://nodei.co/npm/wechat-api.png?downloads=true)](https://www.npmjs.com/package/wechat-api)

[![apidoc](https://npmdoc.github.io/node-npmdoc-wechat-api/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-wechat-api_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-wechat-api/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-wechat-api/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-wechat-api/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jackson Tian"
    },
    "bugs": {
        "url": "https://github.com/node-webot/wechat-api/issues"
    },
    "config": {
        "travis-cov": {
            "threshold": 98
        }
    },
    "dependencies": {
        "formstream": ">=1.0.0",
        "urllib": "2.11.0"
    },
    "description": "微信公共平台Node库 API",
    "devDependencies": {
        "coveralls": "*",
        "expect.js": "*",
        "istanbul": "*",
        "mocha": "*",
        "mocha-lcov-reporter": "*",
        "muk": "*",
        "rewire": "*",
        "travis-cov": "*"
    },
    "directories": {
        "test": "test"
    },
    "dist": {
        "shasum": "2e37d3aa71c1f8f4ea4d1b88f316df90d0618c1b",
        "tarball": "https://registry.npmjs.org/wechat-api/-/wechat-api-1.32.0.tgz"
    },
    "files": [
        "lib",
        "index.js"
    ],
    "gitHead": "b60e04622b8e60e5060620a0bd07561bc14f77fb",
    "homepage": "https://github.com/node-webot/wechat-api#readme",
    "keywords": [
        "weixin",
        "wechat"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "ktmud",
            "email": "jyyjcc@gmail.com"
        },
        {
            "name": "jacksontian",
            "email": "shyvo1987@gmail.com"
        }
    ],
    "name": "wechat-api",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/node-webot/wechat-api.git"
    },
    "scripts": {
        "test": "make test-all"
    },
    "version": "1.32.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module wechat-api](#apidoc.module.wechat-api)
1.  [function <span class="apidocSignatureSpan">wechat-api.</span>AccessToken (accessToken, expireTime)](#apidoc.element.wechat-api.AccessToken)
1.  [function <span class="apidocSignatureSpan">wechat-api.</span>mixin (obj)](#apidoc.element.wechat-api.mixin)
1.  [function <span class="apidocSignatureSpan">wechat-api.</span>patch (functionName, apiUrl, override)](#apidoc.element.wechat-api.patch)
1.  object <span class="apidocSignatureSpan">wechat-api.</span>AccessToken.prototype
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_card
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_custom_service
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_datacube
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_device
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_feedback
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_group
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_ip
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_js
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_mass_send
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_material
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_media
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_menu
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_menu_custom
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_message
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_payment
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_poi
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_qrcode
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_quota
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_semantic
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_shakearound
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_shop_common
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_shop_express
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_shop_goods
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_shop_group
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_shop_order
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_shop_shelf
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_shop_stock
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_tag
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_template
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_url
1.  object <span class="apidocSignatureSpan">wechat-api.</span>api_user
1.  object <span class="apidocSignatureSpan">wechat-api.</span>util

#### [module wechat-api.AccessToken](#apidoc.module.wechat-api.AccessToken)
1.  [function <span class="apidocSignatureSpan">wechat-api.</span>AccessToken (accessToken, expireTime)](#apidoc.element.wechat-api.AccessToken.AccessToken)

#### [module wechat-api.AccessToken.prototype](#apidoc.module.wechat-api.AccessToken.prototype)
1.  [function <span class="apidocSignatureSpan">wechat-api.AccessToken.prototype.</span>isValid ()](#apidoc.element.wechat-api.AccessToken.prototype.isValid)

#### [module wechat-api.api_card](#apidoc.module.wechat-api.api_card)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_activateMembercard (info, callback)](#apidoc.element.wechat-api.api_card._activateMembercard)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_activateMembercardUserForm (info, callback)](#apidoc.element.wechat-api.api_card._activateMembercardUserForm)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_addConsumer (username, locationId, callback)](#apidoc.element.wechat-api.api_card._addConsumer)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_addLocations (locations, callback)](#apidoc.element.wechat-api.api_card._addLocations)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_batchgetSubmerchant (data, callback)](#apidoc.element.wechat-api.api_card._batchgetSubmerchant)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_checkCustomizedCodes (cardId, code, callback)](#apidoc.element.wechat-api.api_card._checkCustomizedCodes)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_checkInBoardingPass (info, callback)](#apidoc.element.wechat-api.api_card._checkInBoardingPass)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_consumeCode (code, cardId, callback)](#apidoc.element.wechat-api.api_card._consumeCode)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_createCard (card, callback)](#apidoc.element.wechat-api.api_card._createCard)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_createCardQRCode (info, expire_seconds, callback)](#apidoc.element.wechat-api.api_card._createCardQRCode)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_createQRCode (card, callback)](#apidoc.element.wechat-api.api_card._createQRCode)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_decryptCode (encryptCode, callback)](#apidoc.element.wechat-api.api_card._decryptCode)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_deleteCard (cardId, callback)](#apidoc.element.wechat-api.api_card._deleteCard)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_getApplyProtocol (callback)](#apidoc.element.wechat-api.api_card._getApplyProtocol)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_getCard (cardId, callback)](#apidoc.element.wechat-api.api_card._getCard)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_getCardDataInfo (cardId, beginDate, endDate, source, callback)](#apidoc.element.wechat-api.api_card._getCardDataInfo)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_getCards (offset, count, status_list, callback)](#apidoc.element.wechat-api.api_card._getCards)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_getCode (code, cardId, callback)](#apidoc.element.wechat-api.api_card._getCode)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_getColors (callback)](#apidoc.element.wechat-api.api_card._getColors)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_getDepositCodesCount (cardId, callback)](#apidoc.element.wechat-api.api_card._getDepositCodesCount)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_getLocations (offset, count, callback)](#apidoc.element.wechat-api.api_card._getLocations)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_getMemberCardUserInfo (info, callback)](#apidoc.element.wechat-api.api_card._getMemberCardUserInfo)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_getMembercard (info, callback)](#apidoc.element.wechat-api.api_card._getMembercard)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_getSubmerchant (merchantId, callback)](#apidoc.element.wechat-api.api_card._getSubmerchant)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_getTotalCardDataInfo (beginDate, endDate, source, callback)](#apidoc.element.wechat-api.api_card._getTotalCardDataInfo)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_importCustomizedCodes (cardId, code, callback)](#apidoc.element.wechat-api.api_card._importCustomizedCodes)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_setTestWhitelist (info, callback)](#apidoc.element.wechat-api.api_card._setTestWhitelist)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_submitSubmerchant (options, callback)](#apidoc.element.wechat-api.api_card._submitSubmerchant)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_unavailableCode (code, cardId, callback)](#apidoc.element.wechat-api.api_card._unavailableCode)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_updateCard (cardId, cardType, cardInfo, callback)](#apidoc.element.wechat-api.api_card._updateCard)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_updateCardStock (cardId, num, callback)](#apidoc.element.wechat-api.api_card._updateCardStock)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_updateCode (code, cardId, newcode, callback)](#apidoc.element.wechat-api.api_card._updateCode)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_updateLuckyMonkeyBalance (code, cardId, balance, callback)](#apidoc.element.wechat-api.api_card._updateLuckyMonkeyBalance)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_updateMeetingTicket (info, callback)](#apidoc.element.wechat-api.api_card._updateMeetingTicket)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_updateMemberCardUserInfo (data, callback)](#apidoc.element.wechat-api.api_card._updateMemberCardUserInfo)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_updateMembercard (info, callback)](#apidoc.element.wechat-api.api_card._updateMembercard)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_updateMovieTicket (info, callback)](#apidoc.element.wechat-api.api_card._updateMovieTicket)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_updateSubmerchant (options, callback)](#apidoc.element.wechat-api.api_card._updateSubmerchant)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_uploadLogo (filepath, callback)](#apidoc.element.wechat-api.api_card._uploadLogo)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>activateMembercard ()](#apidoc.element.wechat-api.api_card.activateMembercard)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>activateMembercardUserForm ()](#apidoc.element.wechat-api.api_card.activateMembercardUserForm)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>addConsumer ()](#apidoc.element.wechat-api.api_card.addConsumer)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>addLocations ()](#apidoc.element.wechat-api.api_card.addLocations)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>batchgetSubmerchant ()](#apidoc.element.wechat-api.api_card.batchgetSubmerchant)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>checkCustomizedCodes ()](#apidoc.element.wechat-api.api_card.checkCustomizedCodes)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>checkInBoardingPass ()](#apidoc.element.wechat-api.api_card.checkInBoardingPass)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>consumeCode ()](#apidoc.element.wechat-api.api_card.consumeCode)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>createCard ()](#apidoc.element.wechat-api.api_card.createCard)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>createCardQRCode ()](#apidoc.element.wechat-api.api_card.createCardQRCode)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>createQRCode ()](#apidoc.element.wechat-api.api_card.createQRCode)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>decryptCode ()](#apidoc.element.wechat-api.api_card.decryptCode)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>deleteCard ()](#apidoc.element.wechat-api.api_card.deleteCard)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>getApplyProtocol ()](#apidoc.element.wechat-api.api_card.getApplyProtocol)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>getCard ()](#apidoc.element.wechat-api.api_card.getCard)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>getCardDataInfo ()](#apidoc.element.wechat-api.api_card.getCardDataInfo)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>getCards ()](#apidoc.element.wechat-api.api_card.getCards)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>getCode ()](#apidoc.element.wechat-api.api_card.getCode)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>getColors ()](#apidoc.element.wechat-api.api_card.getColors)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>getDepositCodesCount ()](#apidoc.element.wechat-api.api_card.getDepositCodesCount)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>getLocations ()](#apidoc.element.wechat-api.api_card.getLocations)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>getMemberCardUserInfo ()](#apidoc.element.wechat-api.api_card.getMemberCardUserInfo)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>getMembercard ()](#apidoc.element.wechat-api.api_card.getMembercard)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>getRedirectUrl (url, encryptCode, cardId)](#apidoc.element.wechat-api.api_card.getRedirectUrl)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>getSubmerchant ()](#apidoc.element.wechat-api.api_card.getSubmerchant)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>getTotalCardDataInfo ()](#apidoc.element.wechat-api.api_card.getTotalCardDataInfo)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>importCustomizedCodes ()](#apidoc.element.wechat-api.api_card.importCustomizedCodes)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>setTestWhitelist ()](#apidoc.element.wechat-api.api_card.setTestWhitelist)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>submitSubmerchant ()](#apidoc.element.wechat-api.api_card.submitSubmerchant)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>unavailableCode ()](#apidoc.element.wechat-api.api_card.unavailableCode)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>updateCard ()](#apidoc.element.wechat-api.api_card.updateCard)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>updateCardStock ()](#apidoc.element.wechat-api.api_card.updateCardStock)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>updateCode ()](#apidoc.element.wechat-api.api_card.updateCode)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>updateLuckyMonkeyBalance ()](#apidoc.element.wechat-api.api_card.updateLuckyMonkeyBalance)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>updateMeetingTicket ()](#apidoc.element.wechat-api.api_card.updateMeetingTicket)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>updateMemberCardUserInfo ()](#apidoc.element.wechat-api.api_card.updateMemberCardUserInfo)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>updateMembercard ()](#apidoc.element.wechat-api.api_card.updateMembercard)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>updateMovieTicket ()](#apidoc.element.wechat-api.api_card.updateMovieTicket)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>updateSubmerchant ()](#apidoc.element.wechat-api.api_card.updateSubmerchant)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_card.</span>uploadLogo ()](#apidoc.element.wechat-api.api_card.uploadLogo)

#### [module wechat-api.api_custom_service](#apidoc.module.wechat-api.api_custom_service)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>_addKfAccount (account, nick, password, callback)](#apidoc.element.wechat-api.api_custom_service._addKfAccount)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>_deleteKfAccount (account, callback)](#apidoc.element.wechat-api.api_custom_service._deleteKfAccount)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>_getCustomServiceList (callback)](#apidoc.element.wechat-api.api_custom_service._getCustomServiceList)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>_getOnlineCustomServiceList (callback)](#apidoc.element.wechat-api.api_custom_service._getOnlineCustomServiceList)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>_getRecords (opts, callback)](#apidoc.element.wechat-api.api_custom_service._getRecords)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>_setKfAccountAvatar (account, filepath, callback)](#apidoc.element.wechat-api.api_custom_service._setKfAccountAvatar)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>_updateKfAccount (account, nick, password, callback)](#apidoc.element.wechat-api.api_custom_service._updateKfAccount)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>addKfAccount ()](#apidoc.element.wechat-api.api_custom_service.addKfAccount)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>deleteKfAccount ()](#apidoc.element.wechat-api.api_custom_service.deleteKfAccount)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>getCustomServiceList ()](#apidoc.element.wechat-api.api_custom_service.getCustomServiceList)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>getOnlineCustomServiceList ()](#apidoc.element.wechat-api.api_custom_service.getOnlineCustomServiceList)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>getRecords ()](#apidoc.element.wechat-api.api_custom_service.getRecords)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>setKfAccountAvatar ()](#apidoc.element.wechat-api.api_custom_service.setKfAccountAvatar)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>updateKfAccount ()](#apidoc.element.wechat-api.api_custom_service.updateKfAccount)

#### [module wechat-api.api_datacube](#apidoc.module.wechat-api.api_datacube)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getArticleSummary (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getArticleSummary)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getArticleTotal (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getArticleTotal)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getInterfaceSummary (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getInterfaceSummary)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getInterfaceSummaryHour (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getInterfaceSummaryHour)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getUpstreamMsg (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getUpstreamMsg)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getUpstreamMsgDist (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getUpstreamMsgDist)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getUpstreamMsgDistMonth (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getUpstreamMsgDistMonth)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getUpstreamMsgDistWeek (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getUpstreamMsgDistWeek)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getUpstreamMsgHour (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getUpstreamMsgHour)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getUpstreamMsgMonth (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getUpstreamMsgMonth)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getUpstreamMsgWeek (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getUpstreamMsgWeek)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getUserCumulate (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getUserCumulate)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getUserRead (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getUserRead)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getUserReadHour (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getUserReadHour)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getUserShare (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getUserShare)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getUserShareHour (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getUserShareHour)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getUserSummary (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getUserSummary)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getArticleSummary (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getArticleSummary)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getArticleTotal (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getArticleTotal)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getInterfaceSummary (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getInterfaceSummary)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getInterfaceSummaryHour (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getInterfaceSummaryHour)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getUpstreamMsg (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getUpstreamMsg)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getUpstreamMsgDist (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getUpstreamMsgDist)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getUpstreamMsgDistMonth (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getUpstreamMsgDistMonth)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getUpstreamMsgDistWeek (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getUpstreamMsgDistWeek)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getUpstreamMsgHour (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getUpstreamMsgHour)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getUpstreamMsgMonth (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getUpstreamMsgMonth)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getUpstreamMsgWeek (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getUpstreamMsgWeek)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getUserCumulate (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getUserCumulate)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getUserRead (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getUserRead)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getUserReadHour (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getUserReadHour)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getUserShare (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getUserShare)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getUserShareHour (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getUserShareHour)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getUserSummary (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getUserSummary)

#### [module wechat-api.api_device](#apidoc.module.wechat-api.api_device)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_device.</span>_authorizeDevices (devices, optype, productid, callback)](#apidoc.element.wechat-api.api_device._authorizeDevices)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_device.</span>_bindDevice (deviceId, openid, ticket, callback)](#apidoc.element.wechat-api.api_device._bindDevice)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_device.</span>_compelBindDevice (deviceId, openid, callback)](#apidoc.element.wechat-api.api_device._compelBindDevice)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_device.</span>_compelUnbindDevice (deviceId, openid, callback)](#apidoc.element.wechat-api.api_device._compelUnbindDevice)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_device.</span>_createDeviceQRCode (deviceIds, callback)](#apidoc.element.wechat-api.api_device._createDeviceQRCode)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_device.</span>_getBindDevice (openid, callback)](#apidoc.element.wechat-api.api_device._getBindDevice)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_device.</span>_getDeviceQRCode (product_id, callback)](#apidoc.element.wechat-api.api_device._getDeviceQRCode)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_device.</span>_getDeviceStatus (deviceId, callback)](#apidoc.element.wechat-api.api_device._getDeviceStatus)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_device.</span>_getOpenID (deviceId, deviceType, callback)](#apidoc.element.wechat-api.api_device._getOpenID)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_device.</span>_transferMessage (deviceType, deviceId, openid, content, callback)](#apidoc.element.wechat-api.api_device._transferMessage)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_device.</span>_transferStatus (deviceType, deviceId, openid, status, callback)](#apidoc.element.wechat-api.api_device._transferStatus)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_device.</span>_unbindDevice (deviceId, openid, ticket, callback)](#apidoc.element.wechat-api.api_device._unbindDevice)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_device.</span>_verifyDeviceQRCode (ticket, callback)](#apidoc.element.wechat-api.api_device._verifyDeviceQRCode)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_device.</span>authorizeDevices ()](#apidoc.element.wechat-api.api_device.authorizeDevices)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_device.</span>bindDevice ()](#apidoc.element.wechat-api.api_device.bindDevice)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_device.</span>compelBindDevice ()](#apidoc.element.wechat-api.api_device.compelBindDevice)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_device.</span>compelUnbindDevice ()](#apidoc.element.wechat-api.api_device.compelUnbindDevice)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_device.</span>createDeviceQRCode ()](#apidoc.element.wechat-api.api_device.createDeviceQRCode)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_device.</span>getBindDevice ()](#apidoc.element.wechat-api.api_device.getBindDevice)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_device.</span>getDeviceQRCode ()](#apidoc.element.wechat-api.api_device.getDeviceQRCode)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_device.</span>getDeviceStatus ()](#apidoc.element.wechat-api.api_device.getDeviceStatus)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_device.</span>getOpenID ()](#apidoc.element.wechat-api.api_device.getOpenID)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_device.</span>transferMessage ()](#apidoc.element.wechat-api.api_device.transferMessage)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_device.</span>transferStatus ()](#apidoc.element.wechat-api.api_device.transferStatus)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_device.</span>unbindDevice ()](#apidoc.element.wechat-api.api_device.unbindDevice)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_device.</span>verifyDeviceQRCode ()](#apidoc.element.wechat-api.api_device.verifyDeviceQRCode)

#### [module wechat-api.api_feedback](#apidoc.module.wechat-api.api_feedback)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_feedback.</span>_updateFeedback (openid, feedbackId, callback)](#apidoc.element.wechat-api.api_feedback._updateFeedback)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_feedback.</span>updateFeedback (openid, feedbackId, callback)](#apidoc.element.wechat-api.api_feedback.updateFeedback)

#### [module wechat-api.api_group](#apidoc.module.wechat-api.api_group)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_group.</span>_createGroup (name, callback)](#apidoc.element.wechat-api.api_group._createGroup)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_group.</span>_getGroups (callback)](#apidoc.element.wechat-api.api_group._getGroups)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_group.</span>_getWhichGroup (openid, callback)](#apidoc.element.wechat-api.api_group._getWhichGroup)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_group.</span>_moveUserToGroup (openid, groupId, callback)](#apidoc.element.wechat-api.api_group._moveUserToGroup)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_group.</span>_removeGroup (groupId, callback)](#apidoc.element.wechat-api.api_group._removeGroup)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_group.</span>_updateGroup (id, name, callback)](#apidoc.element.wechat-api.api_group._updateGroup)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_group.</span>createGroup ()](#apidoc.element.wechat-api.api_group.createGroup)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_group.</span>getGroups ()](#apidoc.element.wechat-api.api_group.getGroups)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_group.</span>getWhichGroup ()](#apidoc.element.wechat-api.api_group.getWhichGroup)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_group.</span>moveUserToGroup ()](#apidoc.element.wechat-api.api_group.moveUserToGroup)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_group.</span>removeGroup ()](#apidoc.element.wechat-api.api_group.removeGroup)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_group.</span>updateGroup ()](#apidoc.element.wechat-api.api_group.updateGroup)

#### [module wechat-api.api_ip](#apidoc.module.wechat-api.api_ip)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_ip.</span>_getIp (callback)](#apidoc.element.wechat-api.api_ip._getIp)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_ip.</span>getIp ()](#apidoc.element.wechat-api.api_ip.getIp)

#### [module wechat-api.api_js](#apidoc.module.wechat-api.api_js)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_js.</span>_getCardExt (param, callback)](#apidoc.element.wechat-api.api_js._getCardExt)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_js.</span>_getJsConfig (param, callback)](#apidoc.element.wechat-api.api_js._getJsConfig)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_js.</span>_getLatestTicket (callback)](#apidoc.element.wechat-api.api_js._getLatestTicket)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_js.</span>_getTicket (type, callback)](#apidoc.element.wechat-api.api_js._getTicket)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_js.</span>getCardExt (param, callback)](#apidoc.element.wechat-api.api_js.getCardExt)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_js.</span>getJsConfig (param, callback)](#apidoc.element.wechat-api.api_js.getJsConfig)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_js.</span>getLatestTicket (callback)](#apidoc.element.wechat-api.api_js.getLatestTicket)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_js.</span>getTicket (type, callback)](#apidoc.element.wechat-api.api_js.getTicket)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_js.</span>registerTicketHandle (getTicketToken, saveTicketToken)](#apidoc.element.wechat-api.api_js.registerTicketHandle)

#### [module wechat-api.api_mass_send](#apidoc.module.wechat-api.api_mass_send)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>_deleteMass (messageId, callback)](#apidoc.element.wechat-api.api_mass_send._deleteMass)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>_getMassMessageStatus (messageId, callback)](#apidoc.element.wechat-api.api_mass_send._getMassMessageStatus)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>_massSend (opts, receivers, callback)](#apidoc.element.wechat-api.api_mass_send._massSend)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>_previewImage (openid, mediaId, callback)](#apidoc.element.wechat-api.api_mass_send._previewImage)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>_previewNews (openid, mediaId, callback)](#apidoc.element.wechat-api.api_mass_send._previewNews)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>_previewText (openid, content, callback)](#apidoc.element.wechat-api.api_mass_send._previewText)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>_previewVideo (openid, mediaId, callback)](#apidoc.element.wechat-api.api_mass_send._previewVideo)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>_previewVoice (openid, mediaId, callback)](#apidoc.element.wechat-api.api_mass_send._previewVoice)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>_uploadMPVideo (opts, callback)](#apidoc.element.wechat-api.api_mass_send._uploadMPVideo)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>_uploadNews (news, callback)](#apidoc.element.wechat-api.api_mass_send._uploadNews)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>deleteMass (messageId, callback)](#apidoc.element.wechat-api.api_mass_send.deleteMass)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>getMassMessageStatus (messageId, callback)](#apidoc.element.wechat-api.api_mass_send.getMassMessageStatus)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>massSend (opts, receivers, callback)](#apidoc.element.wechat-api.api_mass_send.massSend)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>massSendImage (mediaId, receivers, callback)](#apidoc.element.wechat-api.api_mass_send.massSendImage)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>massSendMPVideo (data, receivers, callback)](#apidoc.element.wechat-api.api_mass_send.massSendMPVideo)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>massSendNews (mediaId, receivers, callback)](#apidoc.element.wechat-api.api_mass_send.massSendNews)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>massSendText (content, receivers, callback)](#apidoc.element.wechat-api.api_mass_send.massSendText)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>massSendVideo (mediaId, receivers, callback)](#apidoc.element.wechat-api.api_mass_send.massSendVideo)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>massSendVoice (mediaId, receivers, callback)](#apidoc.element.wechat-api.api_mass_send.massSendVoice)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>previewImage (openid, mediaId, callback)](#apidoc.element.wechat-api.api_mass_send.previewImage)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>previewNews (openid, mediaId, callback)](#apidoc.element.wechat-api.api_mass_send.previewNews)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>previewText (openid, content, callback)](#apidoc.element.wechat-api.api_mass_send.previewText)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>previewVideo (openid, mediaId, callback)](#apidoc.element.wechat-api.api_mass_send.previewVideo)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>previewVoice (openid, mediaId, callback)](#apidoc.element.wechat-api.api_mass_send.previewVoice)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>uploadMPVideo (opts, callback)](#apidoc.element.wechat-api.api_mass_send.uploadMPVideo)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>uploadNews (news, callback)](#apidoc.element.wechat-api.api_mass_send.uploadNews)

#### [module wechat-api.api_material](#apidoc.module.wechat-api.api_material)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_material.</span>_getMaterial (mediaId, callback)](#apidoc.element.wechat-api.api_material._getMaterial)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_material.</span>_getMaterialCount (callback)](#apidoc.element.wechat-api.api_material._getMaterialCount)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_material.</span>_getMaterials (type, offset, count, callback)](#apidoc.element.wechat-api.api_material._getMaterials)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_material.</span>_removeMaterial (mediaId, callback)](#apidoc.element.wechat-api.api_material._removeMaterial)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_material.</span>_updateNewsMaterial (news, callback)](#apidoc.element.wechat-api.api_material._updateNewsMaterial)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_material.</span>_uploadMaterial (filepath, type, callback)](#apidoc.element.wechat-api.api_material._uploadMaterial)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_material.</span>_uploadNewsMaterial (news, callback)](#apidoc.element.wechat-api.api_material._uploadNewsMaterial)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_material.</span>_uploadVideoMaterial (filepath, description, callback)](#apidoc.element.wechat-api.api_material._uploadVideoMaterial)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_material.</span>getMaterial (mediaId, callback)](#apidoc.element.wechat-api.api_material.getMaterial)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_material.</span>getMaterialCount (callback)](#apidoc.element.wechat-api.api_material.getMaterialCount)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_material.</span>getMaterials (type, offset, count, callback)](#apidoc.element.wechat-api.api_material.getMaterials)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_material.</span>removeMaterial (mediaId, callback)](#apidoc.element.wechat-api.api_material.removeMaterial)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_material.</span>updateNewsMaterial (news, callback)](#apidoc.element.wechat-api.api_material.updateNewsMaterial)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_material.</span>uploadImageMaterial (filepath, callback)](#apidoc.element.wechat-api.api_material.uploadImageMaterial)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_material.</span>uploadMaterial ()](#apidoc.element.wechat-api.api_material.uploadMaterial)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_material.</span>uploadNewsMaterial (news, callback)](#apidoc.element.wechat-api.api_material.uploadNewsMaterial)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_material.</span>uploadThumbMaterial (filepath, callback)](#apidoc.element.wechat-api.api_material.uploadThumbMaterial)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_material.</span>uploadVideoMaterial ()](#apidoc.element.wechat-api.api_material.uploadVideoMaterial)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_material.</span>uploadVoiceMaterial (filepath, callback)](#apidoc.element.wechat-api.api_material.uploadVoiceMaterial)

#### [module wechat-api.api_media](#apidoc.module.wechat-api.api_media)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_media.</span>_getMedia (mediaId, callback)](#apidoc.element.wechat-api.api_media._getMedia)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_media.</span>_uploadImage (filepath, callback)](#apidoc.element.wechat-api.api_media._uploadImage)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_media.</span>_uploadImageStream (req, callback)](#apidoc.element.wechat-api.api_media._uploadImageStream)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_media.</span>_uploadMedia (filepath, type, callback)](#apidoc.element.wechat-api.api_media._uploadMedia)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_media.</span>getMedia (mediaId, callback)](#apidoc.element.wechat-api.api_media.getMedia)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_media.</span>uploadImage (filepath, callback)](#apidoc.element.wechat-api.api_media.uploadImage)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_media.</span>uploadImageStream (req, callback)](#apidoc.element.wechat-api.api_media.uploadImageStream)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_media.</span>uploadMedia (filepath, type, callback)](#apidoc.element.wechat-api.api_media.uploadMedia)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_media.</span>uploadThumb (filepath, callback)](#apidoc.element.wechat-api.api_media.uploadThumb)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_media.</span>uploadVideo (filepath, callback)](#apidoc.element.wechat-api.api_media.uploadVideo)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_media.</span>uploadVoice (filepath, callback)](#apidoc.element.wechat-api.api_media.uploadVoice)

#### [module wechat-api.api_menu](#apidoc.module.wechat-api.api_menu)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_menu.</span>_createMenu (menu, callback)](#apidoc.element.wechat-api.api_menu._createMenu)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_menu.</span>_getMenu (callback)](#apidoc.element.wechat-api.api_menu._getMenu)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_menu.</span>_getMenuConfig (callback)](#apidoc.element.wechat-api.api_menu._getMenuConfig)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_menu.</span>_removeMenu (callback)](#apidoc.element.wechat-api.api_menu._removeMenu)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_menu.</span>createMenu (menu, callback)](#apidoc.element.wechat-api.api_menu.createMenu)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_menu.</span>getMenu (callback)](#apidoc.element.wechat-api.api_menu.getMenu)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_menu.</span>getMenuConfig (callback)](#apidoc.element.wechat-api.api_menu.getMenuConfig)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_menu.</span>removeMenu (callback)](#apidoc.element.wechat-api.api_menu.removeMenu)

#### [module wechat-api.api_menu_custom](#apidoc.module.wechat-api.api_menu_custom)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_menu_custom.</span>_createCustomMenu (menu, callback)](#apidoc.element.wechat-api.api_menu_custom._createCustomMenu)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_menu_custom.</span>_removeCustomMenu (menu_id, callback)](#apidoc.element.wechat-api.api_menu_custom._removeCustomMenu)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_menu_custom.</span>_testCustomMenu (user_id, callback)](#apidoc.element.wechat-api.api_menu_custom._testCustomMenu)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_menu_custom.</span>createCustomMenu (menu, callback)](#apidoc.element.wechat-api.api_menu_custom.createCustomMenu)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_menu_custom.</span>removeCustomMenu (menu_id, callback)](#apidoc.element.wechat-api.api_menu_custom.removeCustomMenu)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_menu_custom.</span>testCustomMenu (user_id, callback)](#apidoc.element.wechat-api.api_menu_custom.testCustomMenu)

#### [module wechat-api.api_message](#apidoc.module.wechat-api.api_message)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_message.</span>_sendCard (openid, card, callback)](#apidoc.element.wechat-api.api_message._sendCard)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_message.</span>_sendImage (openid, mediaId, callback)](#apidoc.element.wechat-api.api_message._sendImage)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_message.</span>_sendMpNews (openid, mediaId, callback)](#apidoc.element.wechat-api.api_message._sendMpNews)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_message.</span>_sendMusic (openid, music, callback)](#apidoc.element.wechat-api.api_message._sendMusic)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_message.</span>_sendNews (openid, articles, callback)](#apidoc.element.wechat-api.api_message._sendNews)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_message.</span>_sendText (openid, text, callback)](#apidoc.element.wechat-api.api_message._sendText)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_message.</span>_sendVideo (openid, mediaId, thumbMediaId, callback)](#apidoc.element.wechat-api.api_message._sendVideo)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_message.</span>_sendVoice (openid, mediaId, callback)](#apidoc.element.wechat-api.api_message._sendVoice)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_message.</span>sendCard (openid, card, callback)](#apidoc.element.wechat-api.api_message.sendCard)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_message.</span>sendImage (openid, mediaId, callback)](#apidoc.element.wechat-api.api_message.sendImage)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_message.</span>sendMpNews (openid, mediaId, callback)](#apidoc.element.wechat-api.api_message.sendMpNews)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_message.</span>sendMusic (openid, music, callback)](#apidoc.element.wechat-api.api_message.sendMusic)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_message.</span>sendNews (openid, articles, callback)](#apidoc.element.wechat-api.api_message.sendNews)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_message.</span>sendText (openid, text, callback)](#apidoc.element.wechat-api.api_message.sendText)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_message.</span>sendVideo (openid, mediaId, thumbMediaId, callback)](#apidoc.element.wechat-api.api_message.sendVideo)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_message.</span>sendVoice (openid, mediaId, callback)](#apidoc.element.wechat-api.api_message.sendVoice)

#### [module wechat-api.api_payment](#apidoc.module.wechat-api.api_payment)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_payment.</span>_deliverNotify (data, callback)](#apidoc.element.wechat-api.api_payment._deliverNotify)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_payment.</span>_orderQuery (query, callback)](#apidoc.element.wechat-api.api_payment._orderQuery)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_payment.</span>deliverNotify (data, callback)](#apidoc.element.wechat-api.api_payment.deliverNotify)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_payment.</span>orderQuery (query, callback)](#apidoc.element.wechat-api.api_payment.orderQuery)

#### [module wechat-api.api_poi](#apidoc.module.wechat-api.api_poi)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_poi.</span>_addPoi (poi, callback)](#apidoc.element.wechat-api.api_poi._addPoi)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_poi.</span>_delPoi (poiId, callback)](#apidoc.element.wechat-api.api_poi._delPoi)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_poi.</span>_getPoi (poiId, callback)](#apidoc.element.wechat-api.api_poi._getPoi)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_poi.</span>_getPois (begin, limit, callback)](#apidoc.element.wechat-api.api_poi._getPois)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_poi.</span>_getWXCategory (callback)](#apidoc.element.wechat-api.api_poi._getWXCategory)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_poi.</span>_updatePoi (poi, callback)](#apidoc.element.wechat-api.api_poi._updatePoi)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_poi.</span>addPoi ()](#apidoc.element.wechat-api.api_poi.addPoi)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_poi.</span>delPoi ()](#apidoc.element.wechat-api.api_poi.delPoi)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_poi.</span>getPoi ()](#apidoc.element.wechat-api.api_poi.getPoi)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_poi.</span>getPois ()](#apidoc.element.wechat-api.api_poi.getPois)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_poi.</span>getWXCategory ()](#apidoc.element.wechat-api.api_poi.getWXCategory)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_poi.</span>updatePoi ()](#apidoc.element.wechat-api.api_poi.updatePoi)

#### [module wechat-api.api_qrcode](#apidoc.module.wechat-api.api_qrcode)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_qrcode.</span>_createLimitQRCode (sceneId, callback)](#apidoc.element.wechat-api.api_qrcode._createLimitQRCode)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_qrcode.</span>_createTmpQRCode (sceneId, expire, callback)](#apidoc.element.wechat-api.api_qrcode._createTmpQRCode)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_qrcode.</span>createLimitQRCode (sceneId, callback)](#apidoc.element.wechat-api.api_qrcode.createLimitQRCode)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_qrcode.</span>createTmpQRCode (sceneId, expire, callback)](#apidoc.element.wechat-api.api_qrcode.createTmpQRCode)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_qrcode.</span>showQRCodeURL (ticket)](#apidoc.element.wechat-api.api_qrcode.showQRCodeURL)

#### [module wechat-api.api_quota](#apidoc.module.wechat-api.api_quota)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_quota.</span>_clearQuota (appid, callback)](#apidoc.element.wechat-api.api_quota._clearQuota)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_quota.</span>clearQuota ()](#apidoc.element.wechat-api.api_quota.clearQuota)

#### [module wechat-api.api_semantic](#apidoc.module.wechat-api.api_semantic)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_semantic.</span>_semantic (uid, opts, callback)](#apidoc.element.wechat-api.api_semantic._semantic)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_semantic.</span>semantic (uid, opts, callback)](#apidoc.element.wechat-api.api_semantic.semantic)

#### [module wechat-api.api_shakearound](#apidoc.module.wechat-api.api_shakearound)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_addBeaconGroup (group, callback)](#apidoc.element.wechat-api.api_shakearound._addBeaconGroup)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_addGroupBeacons (options, callback)](#apidoc.element.wechat-api.api_shakearound._addGroupBeacons)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_addLotteryInfo (options, body, callback)](#apidoc.element.wechat-api.api_shakearound._addLotteryInfo)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_applyBeacons (options, callback)](#apidoc.element.wechat-api.api_shakearound._applyBeacons)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_applyBeaconsStatus (apply_id, callback)](#apidoc.element.wechat-api.api_shakearound._applyBeaconsStatus)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_bindBeaconLocation (options, callback)](#apidoc.element.wechat-api.api_shakearound._bindBeaconLocation)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_bindBeaconWithPages (options, callback)](#apidoc.element.wechat-api.api_shakearound._bindBeaconWithPages)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_checkShakeAccountStatus (callback)](#apidoc.element.wechat-api.api_shakearound._checkShakeAccountStatus)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_createPage (page, callback)](#apidoc.element.wechat-api.api_shakearound._createPage)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_deleteBeaconGroup (group_id, callback)](#apidoc.element.wechat-api.api_shakearound._deleteBeaconGroup)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_deleteGroupBeacons (options, callback)](#apidoc.element.wechat-api.api_shakearound._deleteGroupBeacons)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_deletePage (page_id, callback)](#apidoc.element.wechat-api.api_shakearound._deletePage)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_getBeacons (options, callback)](#apidoc.element.wechat-api.api_shakearound._getBeacons)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_getDeviceStatistics (options, callback)](#apidoc.element.wechat-api.api_shakearound._getDeviceStatistics)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_getDeviceStatisticsList (options, callback)](#apidoc.element.wechat-api.api_shakearound._getDeviceStatisticsList)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_getPageStatistics (options, callback)](#apidoc.element.wechat-api.api_shakearound._getPageStatistics)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_getPageStatisticsList (options, callback)](#apidoc.element.wechat-api.api_shakearound._getPageStatisticsList)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_getPages (options, callback)](#apidoc.element.wechat-api.api_shakearound._getPages)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_getShakeInfo (ticket, callback)](#apidoc.element.wechat-api.api_shakearound._getShakeInfo)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_listBeaconGroup (options, callback)](#apidoc.element.wechat-api.api_shakearound._listBeaconGroup)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_queryGroupBeacons (options, callback)](#apidoc.element.wechat-api.api_shakearound._queryGroupBeacons)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_registerShakeAccount (options, callback)](#apidoc.element.wechat-api.api_shakearound._registerShakeAccount)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_searchBeaconPageRelation (options, callback)](#apidoc.element.wechat-api.api_shakearound._searchBeaconPageRelation)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_setLotterySwitch (lotteryId, onoff, callback)](#apidoc.element.wechat-api.api_shakearound._setLotterySwitch)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_setPrizeBucket (options, callback)](#apidoc.element.wechat-api.api_shakearound._setPrizeBucket)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_updateBeacon (options, callback)](#apidoc.element.wechat-api.api_shakearound._updateBeacon)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_updateBeaconGroup (group, callback)](#apidoc.element.wechat-api.api_shakearound._updateBeaconGroup)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_updatePage (page, callback)](#apidoc.element.wechat-api.api_shakearound._updatePage)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_uploadPageIcon (filepath, callback)](#apidoc.element.wechat-api.api_shakearound._uploadPageIcon)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>addBeaconGroup ()](#apidoc.element.wechat-api.api_shakearound.addBeaconGroup)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>addGroupBeacons ()](#apidoc.element.wechat-api.api_shakearound.addGroupBeacons)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>addLotteryInfo ()](#apidoc.element.wechat-api.api_shakearound.addLotteryInfo)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>applyBeacons ()](#apidoc.element.wechat-api.api_shakearound.applyBeacons)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>applyBeaconsStatus ()](#apidoc.element.wechat-api.api_shakearound.applyBeaconsStatus)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>bindBeaconLocation ()](#apidoc.element.wechat-api.api_shakearound.bindBeaconLocation)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>bindBeaconWithPages ()](#apidoc.element.wechat-api.api_shakearound.bindBeaconWithPages)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>checkShakeAccountStatus ()](#apidoc.element.wechat-api.api_shakearound.checkShakeAccountStatus)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>createPage ()](#apidoc.element.wechat-api.api_shakearound.createPage)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>deleteBeaconGroup ()](#apidoc.element.wechat-api.api_shakearound.deleteBeaconGroup)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>deleteGroupBeacons ()](#apidoc.element.wechat-api.api_shakearound.deleteGroupBeacons)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>deletePage ()](#apidoc.element.wechat-api.api_shakearound.deletePage)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>getBeacons ()](#apidoc.element.wechat-api.api_shakearound.getBeacons)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>getDeviceStatistics ()](#apidoc.element.wechat-api.api_shakearound.getDeviceStatistics)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>getDeviceStatisticsList ()](#apidoc.element.wechat-api.api_shakearound.getDeviceStatisticsList)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>getPageStatistics ()](#apidoc.element.wechat-api.api_shakearound.getPageStatistics)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>getPageStatisticsList ()](#apidoc.element.wechat-api.api_shakearound.getPageStatisticsList)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>getPages ()](#apidoc.element.wechat-api.api_shakearound.getPages)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>getShakeInfo ()](#apidoc.element.wechat-api.api_shakearound.getShakeInfo)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>getShakehbConfig (openid, lotteryId, key)](#apidoc.element.wechat-api.api_shakearound.getShakehbConfig)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>listBeaconGroup ()](#apidoc.element.wechat-api.api_shakearound.listBeaconGroup)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>queryGroupBeacons ()](#apidoc.element.wechat-api.api_shakearound.queryGroupBeacons)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>registerShakeAccount ()](#apidoc.element.wechat-api.api_shakearound.registerShakeAccount)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>searchBeaconPageRelation ()](#apidoc.element.wechat-api.api_shakearound.searchBeaconPageRelation)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>setLotterySwitch ()](#apidoc.element.wechat-api.api_shakearound.setLotterySwitch)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>setPrizeBucket ()](#apidoc.element.wechat-api.api_shakearound.setPrizeBucket)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>updateBeacon ()](#apidoc.element.wechat-api.api_shakearound.updateBeacon)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>updateBeaconGroup ()](#apidoc.element.wechat-api.api_shakearound.updateBeaconGroup)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>updatePage ()](#apidoc.element.wechat-api.api_shakearound.updatePage)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>uploadPageIcon ()](#apidoc.element.wechat-api.api_shakearound.uploadPageIcon)

#### [module wechat-api.api_shop_common](#apidoc.module.wechat-api.api_shop_common)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_common.</span>_uploadPicture (filepath, callback)](#apidoc.element.wechat-api.api_shop_common._uploadPicture)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_common.</span>uploadPicture (filepath, callback)](#apidoc.element.wechat-api.api_shop_common.uploadPicture)

#### [module wechat-api.api_shop_express](#apidoc.module.wechat-api.api_shop_express)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_express.</span>_addExpressTemplate (express, callback)](#apidoc.element.wechat-api.api_shop_express._addExpressTemplate)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_express.</span>_deleteExpressTemplate (templateId, callback)](#apidoc.element.wechat-api.api_shop_express._deleteExpressTemplate)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_express.</span>_getAllExpressTemplates (callback)](#apidoc.element.wechat-api.api_shop_express._getAllExpressTemplates)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_express.</span>_getExpressTemplateById (templateId, callback)](#apidoc.element.wechat-api.api_shop_express._getExpressTemplateById)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_express.</span>_updateExpressTemplate (template, callback)](#apidoc.element.wechat-api.api_shop_express._updateExpressTemplate)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_express.</span>addExpressTemplate (express, callback)](#apidoc.element.wechat-api.api_shop_express.addExpressTemplate)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_express.</span>deleteExpressTemplate (templateId, callback)](#apidoc.element.wechat-api.api_shop_express.deleteExpressTemplate)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_express.</span>getAllExpressTemplates (callback)](#apidoc.element.wechat-api.api_shop_express.getAllExpressTemplates)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_express.</span>getExpressTemplateById (templateId, callback)](#apidoc.element.wechat-api.api_shop_express.getExpressTemplateById)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_express.</span>updateExpressTemplate (template, callback)](#apidoc.element.wechat-api.api_shop_express.updateExpressTemplate)

#### [module wechat-api.api_shop_goods](#apidoc.module.wechat-api.api_shop_goods)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>_createGoods (goods, callback)](#apidoc.element.wechat-api.api_shop_goods._createGoods)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>_deleteGoods (productId, callback)](#apidoc.element.wechat-api.api_shop_goods._deleteGoods)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>_getGoods (productId, callback)](#apidoc.element.wechat-api.api_shop_goods._getGoods)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>_getGoodsByStatus (status, callback)](#apidoc.element.wechat-api.api_shop_goods._getGoodsByStatus)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>_getProperties (catId, callback)](#apidoc.element.wechat-api.api_shop_goods._getProperties)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>_getSKUs (catId, callback)](#apidoc.element.wechat-api.api_shop_goods._getSKUs)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>_getSubCats (catId, callback)](#apidoc.element.wechat-api.api_shop_goods._getSubCats)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>_updateGoods (goods, callback)](#apidoc.element.wechat-api.api_shop_goods._updateGoods)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>_updateGoodsStatus (productId, status, callback)](#apidoc.element.wechat-api.api_shop_goods._updateGoodsStatus)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>createGoods (goods, callback)](#apidoc.element.wechat-api.api_shop_goods.createGoods)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>deleteGoods (productId, callback)](#apidoc.element.wechat-api.api_shop_goods.deleteGoods)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>getGoods (productId, callback)](#apidoc.element.wechat-api.api_shop_goods.getGoods)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>getGoodsByStatus (status, callback)](#apidoc.element.wechat-api.api_shop_goods.getGoodsByStatus)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>getProperties (catId, callback)](#apidoc.element.wechat-api.api_shop_goods.getProperties)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>getSKUs (catId, callback)](#apidoc.element.wechat-api.api_shop_goods.getSKUs)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>getSubCats (catId, callback)](#apidoc.element.wechat-api.api_shop_goods.getSubCats)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>updateGoods (goods, callback)](#apidoc.element.wechat-api.api_shop_goods.updateGoods)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>updateGoodsStatus (productId, status, callback)](#apidoc.element.wechat-api.api_shop_goods.updateGoodsStatus)

#### [module wechat-api.api_shop_group](#apidoc.module.wechat-api.api_shop_group)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_group.</span>_createGoodsGroup (groupName, productList, callback)](#apidoc.element.wechat-api.api_shop_group._createGoodsGroup)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_group.</span>_deleteGoodsGroup (groupId, callback)](#apidoc.element.wechat-api.api_shop_group._deleteGoodsGroup)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_group.</span>_getAllGroups (callback)](#apidoc.element.wechat-api.api_shop_group._getAllGroups)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_group.</span>_getGroupById (groupId, callback)](#apidoc.element.wechat-api.api_shop_group._getGroupById)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_group.</span>_updateGoodsForGroup (groupId, addProductList, delProductList, callback)](#apidoc.element.wechat-api.api_shop_group._updateGoodsForGroup)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_group.</span>_updateGoodsGroup (groupId, groupName, callback)](#apidoc.element.wechat-api.api_shop_group._updateGoodsGroup)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_group.</span>createGoodsGroup (groupName, productList, callback)](#apidoc.element.wechat-api.api_shop_group.createGoodsGroup)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_group.</span>deleteGoodsGroup (groupId, callback)](#apidoc.element.wechat-api.api_shop_group.deleteGoodsGroup)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_group.</span>getAllGroups (callback)](#apidoc.element.wechat-api.api_shop_group.getAllGroups)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_group.</span>getGroupById (groupId, callback)](#apidoc.element.wechat-api.api_shop_group.getGroupById)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_group.</span>updateGoodsForGroup (groupId, addProductList, delProductList, callback)](#apidoc.element.wechat-api.api_shop_group.updateGoodsForGroup)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_group.</span>updateGoodsGroup (groupId, groupName, callback)](#apidoc.element.wechat-api.api_shop_group.updateGoodsGroup)

#### [module wechat-api.api_shop_order](#apidoc.module.wechat-api.api_shop_order)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_order.</span>_closeOrder (orderId, callback)](#apidoc.element.wechat-api.api_shop_order._closeOrder)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_order.</span>_getOrderById (orderId, callback)](#apidoc.element.wechat-api.api_shop_order._getOrderById)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_order.</span>_getOrdersByStatus (status, beginTime, endTime, callback)](#apidoc.element.wechat-api.api_shop_order._getOrdersByStatus)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_order.</span>_setExpressForOrder (orderId, deliveryCompany, deliveryTrackNo, callback)](#apidoc.element.wechat-api.api_shop_order._setExpressForOrder)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_order.</span>closeOrder (orderId, callback)](#apidoc.element.wechat-api.api_shop_order.closeOrder)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_order.</span>getOrderById (orderId, callback)](#apidoc.element.wechat-api.api_shop_order.getOrderById)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_order.</span>getOrdersByStatus ()](#apidoc.element.wechat-api.api_shop_order.getOrdersByStatus)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_order.</span>setExpressForOrder (orderId, deliveryCompany, deliveryTrackNo, callback)](#apidoc.element.wechat-api.api_shop_order.setExpressForOrder)

#### [module wechat-api.api_shop_shelf](#apidoc.module.wechat-api.api_shop_shelf)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_shelf.</span>_createShelf (shelf, callback)](#apidoc.element.wechat-api.api_shop_shelf._createShelf)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_shelf.</span>_deleteShelf (shelfId, callback)](#apidoc.element.wechat-api.api_shop_shelf._deleteShelf)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_shelf.</span>_getAllShelves (callback)](#apidoc.element.wechat-api.api_shop_shelf._getAllShelves)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_shelf.</span>_getShelfById (shelfId, callback)](#apidoc.element.wechat-api.api_shop_shelf._getShelfById)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_shelf.</span>_updateShelf (shelf, callback)](#apidoc.element.wechat-api.api_shop_shelf._updateShelf)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_shelf.</span>createShelf (shelf, callback)](#apidoc.element.wechat-api.api_shop_shelf.createShelf)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_shelf.</span>deleteShelf (shelfId, callback)](#apidoc.element.wechat-api.api_shop_shelf.deleteShelf)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_shelf.</span>getAllShelves (callback)](#apidoc.element.wechat-api.api_shop_shelf.getAllShelves)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_shelf.</span>getShelfById (shelfId, callback)](#apidoc.element.wechat-api.api_shop_shelf.getShelfById)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_shelf.</span>updateShelf (shelf, callback)](#apidoc.element.wechat-api.api_shop_shelf.updateShelf)

#### [module wechat-api.api_shop_stock](#apidoc.module.wechat-api.api_shop_stock)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_stock.</span>_updateStock (number, productId, sku, callback)](#apidoc.element.wechat-api.api_shop_stock._updateStock)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_shop_stock.</span>updateStock (number, productId, sku, callback)](#apidoc.element.wechat-api.api_shop_stock.updateStock)

#### [module wechat-api.api_tag](#apidoc.module.wechat-api.api_tag)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>_createTag (name, callback)](#apidoc.element.wechat-api.api_tag._createTag)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>_deleteTag (id, callback)](#apidoc.element.wechat-api.api_tag._deleteTag)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>_editTag (id, name, callback)](#apidoc.element.wechat-api.api_tag._editTag)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>_getTagUsers (tagId, openid, callback)](#apidoc.element.wechat-api.api_tag._getTagUsers)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>_getTags (callback)](#apidoc.element.wechat-api.api_tag._getTags)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>_getUserTags (openid, callback)](#apidoc.element.wechat-api.api_tag._getUserTags)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>_membersBatchtagging (tagId, openList, callback)](#apidoc.element.wechat-api.api_tag._membersBatchtagging)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>_membersBatchuntagging (tagId, openList, callback)](#apidoc.element.wechat-api.api_tag._membersBatchuntagging)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>createTag (name, callback)](#apidoc.element.wechat-api.api_tag.createTag)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>deleteTag (id, callback)](#apidoc.element.wechat-api.api_tag.deleteTag)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>editTag (id, name, callback)](#apidoc.element.wechat-api.api_tag.editTag)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>getTagUsers (tagId, openid, callback)](#apidoc.element.wechat-api.api_tag.getTagUsers)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>getTags (callback)](#apidoc.element.wechat-api.api_tag.getTags)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>getUserTags (openid, callback)](#apidoc.element.wechat-api.api_tag.getUserTags)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>membersBatchtagging (tagId, openList, callback)](#apidoc.element.wechat-api.api_tag.membersBatchtagging)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>membersBatchuntagging (tagId, openList, callback)](#apidoc.element.wechat-api.api_tag.membersBatchuntagging)

#### [module wechat-api.api_template](#apidoc.module.wechat-api.api_template)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_template.</span>_addTemplate (templateIdShort, callback)](#apidoc.element.wechat-api.api_template._addTemplate)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_template.</span>_delPrivateTemplate (templateId, callback)](#apidoc.element.wechat-api.api_template._delPrivateTemplate)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_template.</span>_getAllPrivateTemplate (callback)](#apidoc.element.wechat-api.api_template._getAllPrivateTemplate)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_template.</span>_getIndustry (callback)](#apidoc.element.wechat-api.api_template._getIndustry)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_template.</span>_sendTemplate (openid, templateId, url, data, callback, callback2)](#apidoc.element.wechat-api.api_template._sendTemplate)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_template.</span>_setIndustry (industryIds, callback)](#apidoc.element.wechat-api.api_template._setIndustry)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_template.</span>addTemplate (templateIdShort, callback)](#apidoc.element.wechat-api.api_template.addTemplate)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_template.</span>delPrivateTemplate (templateId, callback)](#apidoc.element.wechat-api.api_template.delPrivateTemplate)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_template.</span>getAllPrivateTemplate (callback)](#apidoc.element.wechat-api.api_template.getAllPrivateTemplate)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_template.</span>getIndustry (callback)](#apidoc.element.wechat-api.api_template.getIndustry)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_template.</span>sendTemplate (openid, templateId, url, data, callback, callback2)](#apidoc.element.wechat-api.api_template.sendTemplate)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_template.</span>setIndustry (industryIds, callback)](#apidoc.element.wechat-api.api_template.setIndustry)

#### [module wechat-api.api_url](#apidoc.module.wechat-api.api_url)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_url.</span>_shorturl (longUrl, callback)](#apidoc.element.wechat-api.api_url._shorturl)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_url.</span>shorturl (longUrl, callback)](#apidoc.element.wechat-api.api_url.shorturl)

#### [module wechat-api.api_user](#apidoc.module.wechat-api.api_user)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_user.</span>_batchGetUsers (openids, callback)](#apidoc.element.wechat-api.api_user._batchGetUsers)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_user.</span>_getFollowers (nextOpenid, callback)](#apidoc.element.wechat-api.api_user._getFollowers)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_user.</span>_getUser (options, callback)](#apidoc.element.wechat-api.api_user._getUser)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_user.</span>_updateRemark (openid, remark, callback)](#apidoc.element.wechat-api.api_user._updateRemark)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_user.</span>batchGetUsers (openids, callback)](#apidoc.element.wechat-api.api_user.batchGetUsers)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_user.</span>getFollowers (nextOpenid, callback)](#apidoc.element.wechat-api.api_user.getFollowers)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_user.</span>getUser (options, callback)](#apidoc.element.wechat-api.api_user.getUser)
1.  [function <span class="apidocSignatureSpan">wechat-api.api_user.</span>updateRemark (openid, remark, callback)](#apidoc.element.wechat-api.api_user.updateRemark)

#### [module wechat-api.util](#apidoc.module.wechat-api.util)
1.  [function <span class="apidocSignatureSpan">wechat-api.util.</span>make (host, name, fn)](#apidoc.element.wechat-api.util.make)
1.  [function <span class="apidocSignatureSpan">wechat-api.util.</span>postJSON (data)](#apidoc.element.wechat-api.util.postJSON)
1.  [function <span class="apidocSignatureSpan">wechat-api.util.</span>wrapper (callback)](#apidoc.element.wechat-api.util.wrapper)



# <a name="apidoc.module.wechat-api"></a>[module wechat-api](#apidoc.module.wechat-api)

#### <a name="apidoc.element.wechat-api.AccessToken"></a>[function <span class="apidocSignatureSpan">wechat-api.</span>AccessToken (accessToken, expireTime)](#apidoc.element.wechat-api.AccessToken)
- description and source-code
```javascript
AccessToken = function (accessToken, expireTime) {
  if (!(this instanceof AccessToken)) {
    return new AccessToken(accessToken, expireTime);
  }
  this.accessToken = accessToken;
  this.expireTime = expireTime;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.mixin"></a>[function <span class="apidocSignatureSpan">wechat-api.</span>mixin (obj)](#apidoc.element.wechat-api.mixin)
- description and source-code
```javascript
mixin = function (obj) {
  for (var key in obj) {
    if (API.prototype.hasOwnProperty(key)) {
      throw new Error('Don\'t allow override existed prototype method. method: '+ key);
    }
    API.prototype[key] = obj[key];
  }
}
```
- example usage
```shell
...



'use strict';

var API = require('./lib/api_common');
// 接口调用频次限制
API.mixin(require('./lib/api_quota'));
// 自定义菜单接口
API.mixin(require('./lib/api_menu'));
// 个性化菜单接口
API.mixin(require('./lib/api_menu_custom'));
// 分组管理
API.mixin(require('./lib/api_group'));
// 标签管理
...
```

#### <a name="apidoc.element.wechat-api.patch"></a>[function <span class="apidocSignatureSpan">wechat-api.</span>patch (functionName, apiUrl, override)](#apidoc.element.wechat-api.patch)
- description and source-code
```javascript
patch = function (functionName, apiUrl, override) {
  if (typeof apiUrl !== 'string') {
    throw new Error('The second argument expect a type of string as the request url of wechat');
  }

  if (typeof functionName !== 'string') {
    throw new Error('The first argument expect a type of string as the name of new function');
  }

  if (API.prototype[functionName] || API.prototype['_' + functionName] ) {
    if (override !== true) {
      throw new Error('wechat-api already has a prototype named ['+ functionName + '], use "true" as third param to override it
or change your new function name.');
    } else {
      console.warn('wechat-api already has a prototype named ['+ functionName + '], will override the orignal one.');
    }
  }

  util.make(API.prototype, functionName, function (info, callback) {
    var hasMark = apiUrl.indexOf('?') >= 0;
    var url = apiUrl + (hasMark ? '&access_token=': '?access_token=') + this.token.accessToken;
    this.request(url, util.postJSON(info), wrapper(callback));
  });
}
```
- example usage
```shell
...
当微信官方文档已更新，但本库未来得及更新，而又想用新的微信 api 时，可调用 patch 方法来扩展新功能。
'''js
var WechatAPI = require('wechat-api');
var api = new WechatAPI(appid, appsecret);

// 扩展新api : updateInfo
// 第一个参数为扩展的新方法名，第二个参数为此 api 调用的微信的 apiurl 地址，会自动加上 token
WechatAPI.patch("updateInfo", "https://api.weixin.qq.com/card/membercard/updateuser");


// 调用刚扩展的方法，与其它 api 接口方法一样。
api.updateInfo(jsonInfo, function (err, data, res) {
  // TODO
});
'''
...
```



# <a name="apidoc.module.wechat-api.AccessToken"></a>[module wechat-api.AccessToken](#apidoc.module.wechat-api.AccessToken)

#### <a name="apidoc.element.wechat-api.AccessToken.AccessToken"></a>[function <span class="apidocSignatureSpan">wechat-api.</span>AccessToken (accessToken, expireTime)](#apidoc.element.wechat-api.AccessToken.AccessToken)
- description and source-code
```javascript
AccessToken = function (accessToken, expireTime) {
  if (!(this instanceof AccessToken)) {
    return new AccessToken(accessToken, expireTime);
  }
  this.accessToken = accessToken;
  this.expireTime = expireTime;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.wechat-api.AccessToken.prototype"></a>[module wechat-api.AccessToken.prototype](#apidoc.module.wechat-api.AccessToken.prototype)

#### <a name="apidoc.element.wechat-api.AccessToken.prototype.isValid"></a>[function <span class="apidocSignatureSpan">wechat-api.AccessToken.prototype.</span>isValid ()](#apidoc.element.wechat-api.AccessToken.prototype.isValid)
- description and source-code
```javascript
isValid = function () {
  return !!this.accessToken && (new Date().getTime()) < this.expireTime;
}
```
- example usage
```shell
...
// 调用用户传入的获取ticket的异步方法，获得ticket之后使用（并缓存它）。
that.getTicketToken('jsapi', function (err, cache) {
  if (err) {
    return callback(err);
  }
  var ticket;
  // 有ticket并且ticket有效直接调用
  if (cache && (ticket = new Ticket(cache.ticket, cache.expireTime)).isValid()) {
    // 暂时保存ticket
    that.jsTicket = ticket;
    if (!retryed) {
      var retryHandle = function (err, data, res) {
        // 重试
        if (data && data.errcode && data.errcode === INVALID_TICKET_CODE) {
          return preRequestJSApi.call(that, method, args, true);
...
```



# <a name="apidoc.module.wechat-api.api_card"></a>[module wechat-api.api_card](#apidoc.module.wechat-api.api_card)

#### <a name="apidoc.element.wechat-api.api_card._activateMembercard"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_activateMembercard (info, callback)](#apidoc.element.wechat-api.api_card._activateMembercard)
- description and source-code
```javascript
_activateMembercard = function (info, callback) {
  var url = this.endpoint + '/card/membercard/activate?access_token=' + this.token.accessToken;
  this.request(url, postJSON(info), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._activateMembercardUserForm"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_activateMembercardUserForm (info, callback)](#apidoc.element.wechat-api.api_card._activateMembercardUserForm)
- description and source-code
```javascript
_activateMembercardUserForm = function (info, callback) {
  var url = this.endpoint + '/card/membercard/activateuserform/set?access_token=' + this.token.accessToken;
  this.request(url, postJSON(info), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._addConsumer"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_addConsumer (username, locationId, callback)](#apidoc.element.wechat-api.api_card._addConsumer)
- description and source-code
```javascript
_addConsumer = function (username, locationId, callback) {
  var url = this.endpoint + '/card/consumer/add?access_token=' + this.token.accessToken;
  var data = {
    'username': username,
    'is_super_consumer': true
  };
  if (locationId) {
    data.location_id = locationId;
    data.is_super_consumer = false;
  }
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._addLocations"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_addLocations (locations, callback)](#apidoc.element.wechat-api.api_card._addLocations)
- description and source-code
```javascript
_addLocations = function (locations, callback) {
  var data = {
    location_list: locations
  };
  var url = this.endpoint + '/card/location/batchadd?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._batchgetSubmerchant"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_batchgetSubmerchant (data, callback)](#apidoc.element.wechat-api.api_card._batchgetSubmerchant)
- description and source-code
```javascript
_batchgetSubmerchant = function (data, callback) {
  var url = this.endpoint + '/card/submerchant/batchget?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._checkCustomizedCodes"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_checkCustomizedCodes (cardId, code, callback)](#apidoc.element.wechat-api.api_card._checkCustomizedCodes)
- description and source-code
```javascript
_checkCustomizedCodes = function (cardId, code, callback) {
  var url = this.endpoint + '/card/code/checkcode?access_token=' + this.token.accessToken;
  var data = {
    'card_id': cardId,
    'code': code
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._checkInBoardingPass"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_checkInBoardingPass (info, callback)](#apidoc.element.wechat-api.api_card._checkInBoardingPass)
- description and source-code
```javascript
_checkInBoardingPass = function (info, callback) {
  var url = this.endpoint + '/card/boardingpass/checkin?access_token=' + this.token.accessToken;
  this.request(url, postJSON(info), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._consumeCode"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_consumeCode (code, cardId, callback)](#apidoc.element.wechat-api.api_card._consumeCode)
- description and source-code
```javascript
_consumeCode = function (code, cardId, callback) {
  var url = this.endpoint + '/card/code/consume?access_token=' + this.token.accessToken;
  var data = {
    code: code,
    card_id: cardId
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._createCard"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_createCard (card, callback)](#apidoc.element.wechat-api.api_card._createCard)
- description and source-code
```javascript
_createCard = function (card, callback) {
  var url = this.endpoint + '/card/create?access_token=' + this.token.accessToken;
  var data = {card: card};
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._createCardQRCode"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_createCardQRCode (info, expire_seconds, callback)](#apidoc.element.wechat-api.api_card._createCardQRCode)
- description and source-code
```javascript
_createCardQRCode = function (info, expire_seconds, callback) {
  if(typeof expire_seconds === 'function') {
    callback = expire_seconds;
    expire_seconds = null;
  }
  var url = this.endpoint + '/card/qrcode/create?access_token=' + this.token.accessToken;
  var data = {
    action_name: 'QR_'+Object.keys(info)[0].toUpperCase(),
    expire_seconds: expire_seconds,
    action_info: info
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._createQRCode"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_createQRCode (card, callback)](#apidoc.element.wechat-api.api_card._createQRCode)
- description and source-code
```javascript
_createQRCode = function (card, callback) {
  var url = this.endpoint + '/card/qrcode/create?access_token=' + this.token.accessToken;
  var data = {
    action_name: 'QR_CARD',
    action_info: {
      card: card
    }
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._decryptCode"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_decryptCode (encryptCode, callback)](#apidoc.element.wechat-api.api_card._decryptCode)
- description and source-code
```javascript
_decryptCode = function (encryptCode, callback) {
  var url = this.endpoint + '/card/code/decrypt?access_token=' + this.token.accessToken;
  var data = {
    encrypt_code: encryptCode
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._deleteCard"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_deleteCard (cardId, callback)](#apidoc.element.wechat-api.api_card._deleteCard)
- description and source-code
```javascript
_deleteCard = function (cardId, callback) {
  var url = this.endpoint + '/card/delete?access_token=' + this.token.accessToken;
  var data = {
    card_id: cardId
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._getApplyProtocol"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_getApplyProtocol (callback)](#apidoc.element.wechat-api.api_card._getApplyProtocol)
- description and source-code
```javascript
_getApplyProtocol = function (callback) {
  var url = this.endpoint + '/card/getapplyprotocol?access_token=' + this.token.accessToken;
  this.request(url, {dataType: 'json'}, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._getCard"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_getCard (cardId, callback)](#apidoc.element.wechat-api.api_card._getCard)
- description and source-code
```javascript
_getCard = function (cardId, callback) {
  var url = this.endpoint + '/card/get?access_token=' + this.token.accessToken;
  var data = {
    card_id: cardId
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._getCardDataInfo"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_getCardDataInfo (cardId, beginDate, endDate, source, callback)](#apidoc.element.wechat-api.api_card._getCardDataInfo)
- description and source-code
```javascript
_getCardDataInfo = function (cardId, beginDate, endDate, source, callback) {
  var url = this.endpoint + '/datacube/getcardcardinfo?access_token=' + this.token.accessToken;
  var data = {
    'begin_date': beginDate,
    'end_date': endDate,
    'cond_source': source,
    'card_id': cardId
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._getCards"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_getCards (offset, count, status_list, callback)](#apidoc.element.wechat-api.api_card._getCards)
- description and source-code
```javascript
_getCards = function (offset, count, status_list, callback) {
  var url = this.endpoint + '/card/batchget?access_token=' + this.token.accessToken;
  var data = {
    offset: offset,
    count: count
  };
  if (typeof status_list !== 'function') {
    data.status_list = status_list;
  } else {
    callback = status_list;
  }
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._getCode"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_getCode (code, cardId, callback)](#apidoc.element.wechat-api.api_card._getCode)
- description and source-code
```javascript
_getCode = function (code, cardId, callback) {
  var url = this.endpoint + '/card/code/get?access_token=' + this.token.accessToken;
  var data = {
    code: code
  };
  if (typeof cardId !== 'function') {
    data.card_id = cardId;
  } else {
    callback = cardId;
  }
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._getColors"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_getColors (callback)](#apidoc.element.wechat-api.api_card._getColors)
- description and source-code
```javascript
_getColors = function (callback) {
  var url = this.endpoint + '/card/getcolors?access_token=' + this.token.accessToken;
  this.request(url, {dataType: 'json'}, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._getDepositCodesCount"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_getDepositCodesCount (cardId, callback)](#apidoc.element.wechat-api.api_card._getDepositCodesCount)
- description and source-code
```javascript
_getDepositCodesCount = function (cardId, callback) {
  var url = this.endpoint + '/card/code/getdepositcount?access_token=' + this.token.accessToken;
  var data = {
    'card_id': cardId
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._getLocations"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_getLocations (offset, count, callback)](#apidoc.element.wechat-api.api_card._getLocations)
- description and source-code
```javascript
_getLocations = function (offset, count, callback) {
  var data = {
    offset: offset,
    count: count
  };
  var url = this.endpoint + '/card/location/batchget?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._getMemberCardUserInfo"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_getMemberCardUserInfo (info, callback)](#apidoc.element.wechat-api.api_card._getMemberCardUserInfo)
- description and source-code
```javascript
_getMemberCardUserInfo = function (info, callback) {
  var url = this.endpoint + '/card/membercard/userinfo/get?access_token=' + this.token.accessToken;
  var data = info;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._getMembercard"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_getMembercard (info, callback)](#apidoc.element.wechat-api.api_card._getMembercard)
- description and source-code
```javascript
_getMembercard = function (info, callback) {
  var url = this.endpoint + '/card/membercard/userinfo/get?access_token=' + this.token.accessToken;
  this.request(url, postJSON(info), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._getSubmerchant"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_getSubmerchant (merchantId, callback)](#apidoc.element.wechat-api.api_card._getSubmerchant)
- description and source-code
```javascript
_getSubmerchant = function (merchantId, callback) {
  var url = this.endpoint + '/card/submerchant/get?access_token=' + this.token.accessToken;
  var data = {
    'merchant_id': merchantId
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._getTotalCardDataInfo"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_getTotalCardDataInfo (beginDate, endDate, source, callback)](#apidoc.element.wechat-api.api_card._getTotalCardDataInfo)
- description and source-code
```javascript
_getTotalCardDataInfo = function (beginDate, endDate, source, callback) {
  var url = this.endpoint + '/datacube/getcardbizuininfo?access_token=' + this.token.accessToken;
  var data = {
    'begin_date': beginDate,
    'end_date': endDate,
    'cond_source': source
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._importCustomizedCodes"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_importCustomizedCodes (cardId, code, callback)](#apidoc.element.wechat-api.api_card._importCustomizedCodes)
- description and source-code
```javascript
_importCustomizedCodes = function (cardId, code, callback) {
  var url = this.endpoint + '/card/code/deposit?access_token=' + this.token.accessToken;
  var data = {
    'card_id': cardId,
    'code': code
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._setTestWhitelist"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_setTestWhitelist (info, callback)](#apidoc.element.wechat-api.api_card._setTestWhitelist)
- description and source-code
```javascript
_setTestWhitelist = function (info, callback) {
  var url = this.endpoint + '/card/testwhitelist/set?access_token=' + this.token.accessToken;
  this.request(url, postJSON(info), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._submitSubmerchant"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_submitSubmerchant (options, callback)](#apidoc.element.wechat-api.api_card._submitSubmerchant)
- description and source-code
```javascript
_submitSubmerchant = function (options, callback) {
  var url = this.endpoint + '/card/submerchant/submit?access_token=' + this.token.accessToken;
  var data = {
    'info': options
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._unavailableCode"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_unavailableCode (code, cardId, callback)](#apidoc.element.wechat-api.api_card._unavailableCode)
- description and source-code
```javascript
_unavailableCode = function (code, cardId, callback) {
  var url = this.endpoint + '/card/code/unavailable?access_token=' + this.token.accessToken;
  var data = {
    code: code
  };
  if (typeof cardId !== 'function') {
    data.card_id = cardId;
  } else {
    callback = cardId;
  }
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._updateCard"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_updateCard (cardId, cardType, cardInfo, callback)](#apidoc.element.wechat-api.api_card._updateCard)
- description and source-code
```javascript
_updateCard = function (cardId, cardType, cardInfo, callback) {
  var url = this.endpoint + '/card/update?access_token=' + this.token.accessToken;
  var data = {
    card_id: cardId
  };
  data[cardType.toLowerCase()] = cardInfo;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._updateCardStock"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_updateCardStock (cardId, num, callback)](#apidoc.element.wechat-api.api_card._updateCardStock)
- description and source-code
```javascript
_updateCardStock = function (cardId, num, callback) {
  var url = this.endpoint + '/card/modifystock?access_token=' + this.token.accessToken;
  var data = {
    card_id: cardId
  };
  if (num > 0) {
    data.increase_stock_value = Math.abs(num);
  } else {
    data.reduce_stock_value = Math.abs(num);
  }
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._updateCode"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_updateCode (code, cardId, newcode, callback)](#apidoc.element.wechat-api.api_card._updateCode)
- description and source-code
```javascript
_updateCode = function (code, cardId, newcode, callback) {
  var url = this.endpoint + '/card/code/update?access_token=' + this.token.accessToken;
  var data = {
    code: code,
    card_id: cardId,
    newcode: newcode
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._updateLuckyMonkeyBalance"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_updateLuckyMonkeyBalance (code, cardId, balance, callback)](#apidoc.element.wechat-api.api_card._updateLuckyMonkeyBalance)
- description and source-code
```javascript
_updateLuckyMonkeyBalance = function (code, cardId, balance, callback) {
  var url = this.endpoint + '/card/luckymonkey/updateuserbalance?access_token=' + this.token.accessToken;
  var data = {
    'code': code,
    'card_id': cardId,
    'balance': balance
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._updateMeetingTicket"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_updateMeetingTicket (info, callback)](#apidoc.element.wechat-api.api_card._updateMeetingTicket)
- description and source-code
```javascript
_updateMeetingTicket = function (info, callback) {
  var url = this.endpoint + '/card/meetingticket/updateuser?access_token=' + this.token.accessToken;
  this.request(url, postJSON(info), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._updateMemberCardUserInfo"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_updateMemberCardUserInfo (data, callback)](#apidoc.element.wechat-api.api_card._updateMemberCardUserInfo)
- description and source-code
```javascript
_updateMemberCardUserInfo = function (data, callback) {
  var url = this.endpoint + '/card/membercard/updateuser?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._updateMembercard"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_updateMembercard (info, callback)](#apidoc.element.wechat-api.api_card._updateMembercard)
- description and source-code
```javascript
_updateMembercard = function (info, callback) {
  var url = this.endpoint + '/card/membercard/updateuser?access_token=' + this.token.accessToken;
  this.request(url, postJSON(info), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._updateMovieTicket"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_updateMovieTicket (info, callback)](#apidoc.element.wechat-api.api_card._updateMovieTicket)
- description and source-code
```javascript
_updateMovieTicket = function (info, callback) {
  var url = this.endpoint + '/card/movieticket/updateuser?access_token=' + this.token.accessToken;
  this.request(url, postJSON(info), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._updateSubmerchant"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_updateSubmerchant (options, callback)](#apidoc.element.wechat-api.api_card._updateSubmerchant)
- description and source-code
```javascript
_updateSubmerchant = function (options, callback) {
  var url = this.endpoint + '/card/submerchant/update?access_token=' + this.token.accessToken;
  var data = {
    'info': options
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card._uploadLogo"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>_uploadLogo (filepath, callback)](#apidoc.element.wechat-api.api_card._uploadLogo)
- description and source-code
```javascript
_uploadLogo = function (filepath, callback) {
  var that = this;
  fs.stat(filepath, function (err, stat) {
    if (err) {
      return callback(err);
    }
    var form = formstream();
    form.file('buffer', filepath, path.basename(filepath), stat.size);
    var url = that.fileServerPrefix + 'media/uploadimg?access_token=' + that.token.accessToken;
    var opts = {
      dataType: 'json',
      type: 'POST',
      timeout: 60000, // 60秒超时
      headers: form.headers(),
      stream: form
    };
    that.request(url, opts, wrapper(callback));
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card.activateMembercard"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>activateMembercard ()](#apidoc.element.wechat-api.api_card.activateMembercard)
- description and source-code
```javascript
activateMembercard = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card.activateMembercardUserForm"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>activateMembercardUserForm ()](#apidoc.element.wechat-api.api_card.activateMembercardUserForm)
- description and source-code
```javascript
activateMembercardUserForm = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
});

/**
* 设置开卡字段接口
* '''
* Examples:
* '''
* api.activateMembercardUserForm(info, callback);
*
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
...
```

#### <a name="apidoc.element.wechat-api.api_card.addConsumer"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>addConsumer ()](#apidoc.element.wechat-api.api_card.addConsumer)
- description and source-code
```javascript
addConsumer = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...

/**
* 设置商户的核销员
* 接口说明
* 开发者需调用该接口设置商户的核销员,并指定核销员的门店。
* Examples:
* '''
* api.addConsumer('username', 'locationId', callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_card.addLocations"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>addLocations ()](#apidoc.element.wechat-api.api_card.addLocations)
- description and source-code
```javascript
addLocations = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card.batchgetSubmerchant"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>batchgetSubmerchant ()](#apidoc.element.wechat-api.api_card.batchgetSubmerchant)
- description and source-code
```javascript
batchgetSubmerchant = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...

/**
* 批量拉取子商户信息接口
* 接口说明
* 母商户可以通过该接口批量拉取子商户的相关信息，一次调用最多拉取100个子商户的信息，可以通过多次拉去满足不同的查询需求
* Examples:
* '''
* api.batchgetSubmerchant(data, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* @name batchgetSubmerchant
...
```

#### <a name="apidoc.element.wechat-api.api_card.checkCustomizedCodes"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>checkCustomizedCodes ()](#apidoc.element.wechat-api.api_card.checkCustomizedCodes)
- description and source-code
```javascript
checkCustomizedCodes = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
*   "11111",
*   "22222",
*   "33333"
* ]
* '''
* Examples:
* '''
* api.checkCustomizedCodes('cardId', code, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_card.checkInBoardingPass"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>checkInBoardingPass ()](#apidoc.element.wechat-api.api_card.checkInBoardingPass)
- description and source-code
```javascript
checkInBoardingPass = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card.consumeCode"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>consumeCode ()](#apidoc.element.wechat-api.api_card.consumeCode)
- description and source-code
```javascript
consumeCode = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card.createCard"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>createCard ()](#apidoc.element.wechat-api.api_card.createCard)
- description and source-code
```javascript
createCard = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card.createCardQRCode"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>createCardQRCode ()](#apidoc.element.wechat-api.api_card.createCardQRCode)
- description and source-code
```javascript
createCardQRCode = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
 this.request(url, postJSON(data), wrapper(callback));
});

/**
* 创建用于投放的卡卷二维码，支持投放单张卡卷和多张卡卷
* Examples:
* '''
* api.createCardQRCode('info', 'expire_seconds', callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_card.createQRCode"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>createQRCode ()](#apidoc.element.wechat-api.api_card.createQRCode)
- description and source-code
```javascript
createQRCode = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card.decryptCode"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>decryptCode ()](#apidoc.element.wechat-api.api_card.decryptCode)
- description and source-code
```javascript
decryptCode = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card.deleteCard"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>deleteCard ()](#apidoc.element.wechat-api.api_card.deleteCard)
- description and source-code
```javascript
deleteCard = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card.getApplyProtocol"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>getApplyProtocol ()](#apidoc.element.wechat-api.api_card.getApplyProtocol)
- description and source-code
```javascript
getApplyProtocol = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
* 接口说明
* 通过调用该接口查询卡券开放的类目ID，类目会随业务发展变更，请每次用接口去查询获取实时卡券类目。
* 注意：
* 1. 本接口查询的返回值还有卡券资质ID,此处的卡券资质为：已微信认证的公众号通过微信公众平台申请卡券功能时，所需的资质。
* 2.对于第三方开发者代制（无公众号）模式，子商户无论选择什么类目，均暂不需按照此返回提供资质，返回值仅参考类目ID 即可。
* Examples:
* '''
* api.getApplyProtocol(callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_card.getCard"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>getCard ()](#apidoc.element.wechat-api.api_card.getCard)
- description and source-code
```javascript
getCard = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card.getCardDataInfo"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>getCardDataInfo ()](#apidoc.element.wechat-api.api_card.getCardDataInfo)
- description and source-code
```javascript
getCardDataInfo = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card.getCards"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>getCards ()](#apidoc.element.wechat-api.api_card.getCards)
- description and source-code
```javascript
getCards = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card.getCode"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>getCode ()](#apidoc.element.wechat-api.api_card.getCode)
- description and source-code
```javascript
getCode = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card.getColors"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>getColors ()](#apidoc.element.wechat-api.api_card.getColors)
- description and source-code
```javascript
getColors = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card.getDepositCodesCount"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>getDepositCodesCount ()](#apidoc.element.wechat-api.api_card.getDepositCodesCount)
- description and source-code
```javascript
getDepositCodesCount = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...

/**
* 查询导入code数目接口
* 接口说明
* 支持开发者调用该接口查询code导入微信后台成功的数目。
* Examples:
* '''
* api.getDepositCodesCount('cardId', callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_card.getLocations"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>getLocations ()](#apidoc.element.wechat-api.api_card.getLocations)
- description and source-code
```javascript
getLocations = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card.getMemberCardUserInfo"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>getMemberCardUserInfo ()](#apidoc.element.wechat-api.api_card.getMemberCardUserInfo)
- description and source-code
```javascript
getMemberCardUserInfo = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...

/**
* 拉取拉取会员信息接口
* 接口说明
* 支持开发者根据CardID和Code查询会员信息。
* Examples:
* '''
* api.getMemberCardUserInfo({"card_id": abd5e78412e5d12ff,"code": 5566778811002233}, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* @name getMemberCardUserInfo
...
```

#### <a name="apidoc.element.wechat-api.api_card.getMembercard"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>getMembercard ()](#apidoc.element.wechat-api.api_card.getMembercard)
- description and source-code
```javascript
getMembercard = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card.getRedirectUrl"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>getRedirectUrl (url, encryptCode, cardId)](#apidoc.element.wechat-api.api_card.getRedirectUrl)
- description and source-code
```javascript
getRedirectUrl = function (url, encryptCode, cardId) {
  // TODO
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card.getSubmerchant"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>getSubmerchant ()](#apidoc.element.wechat-api.api_card.getSubmerchant)
- description and source-code
```javascript
getSubmerchant = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
/**
* 拉取单个子商户信息接口
* 接口说明
* 通过指定的子商户merchant_id，拉取该子商户的基础信息。
* 注意，用母商户去调用接口，但接口内传入的是子商户的merchant_id。
* Examples:
* '''
* api.getSubmerchant('merchantId', callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* @name getSubmerchant
...
```

#### <a name="apidoc.element.wechat-api.api_card.getTotalCardDataInfo"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>getTotalCardDataInfo ()](#apidoc.element.wechat-api.api_card.getTotalCardDataInfo)
- description and source-code
```javascript
getTotalCardDataInfo = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card.importCustomizedCodes"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>importCustomizedCodes ()](#apidoc.element.wechat-api.api_card.importCustomizedCodes)
- description and source-code
```javascript
importCustomizedCodes = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
*   "11111",
*   "22222",
*   "33333"
* ]
* '''
* Examples:
* '''
* api.importCustomizedCodes('cardId', code, callback);
*
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
...
```

#### <a name="apidoc.element.wechat-api.api_card.setTestWhitelist"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>setTestWhitelist ()](#apidoc.element.wechat-api.api_card.setTestWhitelist)
- description and source-code
```javascript
setTestWhitelist = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card.submitSubmerchant"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>submitSubmerchant ()](#apidoc.element.wechat-api.api_card.submitSubmerchant)
- description and source-code
```javascript
submitSubmerchant = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
/**
* 创建子商户接口
* 接口说明
* 支持母商户调用该接口传入子商户的相关资料，并获取子商户ID，用于子商户的卡券功能管理。
* 子商户的资质包括：商户名称、商户logo（图片）、卡券类目、授权函（扫描件或彩照）、授权函有效期截止时间。
* Examples:
* '''
* api.submitSubmerchant(options, callback);
* '''
* options:
* {
*  "brand_name": "aaaaaa",
*  "app_id"："xxxxxxxxxxx",
*  "logo_url": "http://mmbiz.xxxx",
*  "protocol": "xxxxxxxxxx",
...
```

#### <a name="apidoc.element.wechat-api.api_card.unavailableCode"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>unavailableCode ()](#apidoc.element.wechat-api.api_card.unavailableCode)
- description and source-code
```javascript
unavailableCode = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card.updateCard"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>updateCard ()](#apidoc.element.wechat-api.api_card.updateCard)
- description and source-code
```javascript
updateCard = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card.updateCardStock"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>updateCardStock ()](#apidoc.element.wechat-api.api_card.updateCardStock)
- description and source-code
```javascript
updateCardStock = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card.updateCode"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>updateCode ()](#apidoc.element.wechat-api.api_card.updateCode)
- description and source-code
```javascript
updateCode = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card.updateLuckyMonkeyBalance"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>updateLuckyMonkeyBalance ()](#apidoc.element.wechat-api.api_card.updateLuckyMonkeyBalance)
- description and source-code
```javascript
updateLuckyMonkeyBalance = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card.updateMeetingTicket"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>updateMeetingTicket ()](#apidoc.element.wechat-api.api_card.updateMeetingTicket)
- description and source-code
```javascript
updateMeetingTicket = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card.updateMemberCardUserInfo"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>updateMemberCardUserInfo ()](#apidoc.element.wechat-api.api_card.updateMemberCardUserInfo)
- description and source-code
```javascript
updateMemberCardUserInfo = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...

/**
* 更新会员信息
* 接口说明
* 当会员持卡消费后，支持开发者调用该接口更新会员信息。会员卡交易后的每次信息变更需通过该接口通知微信，便于后续消息通知及其他扩展功能。
* Examples:
* '''
* api.updateMemberCardUserInfo(data, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* @name getMemberCardUserInfo
...
```

#### <a name="apidoc.element.wechat-api.api_card.updateMembercard"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>updateMembercard ()](#apidoc.element.wechat-api.api_card.updateMembercard)
- description and source-code
```javascript
updateMembercard = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card.updateMovieTicket"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>updateMovieTicket ()](#apidoc.element.wechat-api.api_card.updateMovieTicket)
- description and source-code
```javascript
updateMovieTicket = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_card.updateSubmerchant"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>updateSubmerchant ()](#apidoc.element.wechat-api.api_card.updateSubmerchant)
- description and source-code
```javascript
updateSubmerchant = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...

/**
* 更新子商户接口
* 接口说明
* 支持调用该接口更新子商户信息。
* Examples:
* '''
* api.updateSubmerchant(options, callback);
* '''
* options:
* {
*  "merchant_id": 12,
*  "brand_name": "aaaaaa",
*  "app_id"："xxxxxxxxxxx",
*  "logo_url": "http://mmbiz.xxxx",
...
```

#### <a name="apidoc.element.wechat-api.api_card.uploadLogo"></a>[function <span class="apidocSignatureSpan">wechat-api.api_card.</span>uploadLogo ()](#apidoc.element.wechat-api.api_card.uploadLogo)
- description and source-code
```javascript
uploadLogo = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
var postJSON = util.postJSON;
var make = util.make;

/**
* 上传Logo
* Examples:
* '''
* api.uploadLogo('filepath', callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```



# <a name="apidoc.module.wechat-api.api_custom_service"></a>[module wechat-api.api_custom_service](#apidoc.module.wechat-api.api_custom_service)

#### <a name="apidoc.element.wechat-api.api_custom_service._addKfAccount"></a>[function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>_addKfAccount (account, nick, password, callback)](#apidoc.element.wechat-api.api_custom_service._addKfAccount)
- description and source-code
```javascript
_addKfAccount = function (account, nick, password, callback) {
  // https://api.weixin.qq.com/customservice/kfaccount/add?access_token=ACCESS_TOKEN
  var url = this.endpoint + '/customservice/kfaccount/add?access_token=' + this.token.accessToken;
  var data = {
    'kf_account': account,
    'nickname': nick,
    'password': md5(password)
  };

  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_custom_service._deleteKfAccount"></a>[function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>_deleteKfAccount (account, callback)](#apidoc.element.wechat-api.api_custom_service._deleteKfAccount)
- description and source-code
```javascript
_deleteKfAccount = function (account, callback) {
  // https://api.weixin.qq.com/customservice/kfaccount/del?access_token=ACCESS_TOKEN
  var url = this.endpoint + '/customservice/kfaccount/del?access_token=' + this.token.accessToken + '&kf_account=' + account;
  this.request(url, {dataType: 'json'}, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_custom_service._getCustomServiceList"></a>[function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>_getCustomServiceList (callback)](#apidoc.element.wechat-api.api_custom_service._getCustomServiceList)
- description and source-code
```javascript
_getCustomServiceList = function (callback) {
  // https://api.weixin.qq.com/cgi-bin/customservice/getkflist?access_token= ACCESS_TOKEN
  var url = this.endpoint + '/cgi-bin/customservice/getkflist?access_token=' + this.token.accessToken;
  this.request(url, {dataType: 'json'}, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_custom_service._getOnlineCustomServiceList"></a>[function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>_getOnlineCustomServiceList (callback)](#apidoc.element.wechat-api.api_custom_service._getOnlineCustomServiceList)
- description and source-code
```javascript
_getOnlineCustomServiceList = function (callback) {
  // https://api.weixin.qq.com/cgi-bin/customservice/getonlinekflist?access_token= ACCESS_TOKEN
  var url = this.endpoint + '/cgi-bin/customservice/getonlinekflist?access_token=' + this.token.accessToken;
  this.request(url, {dataType: 'json'}, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_custom_service._getRecords"></a>[function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>_getRecords (opts, callback)](#apidoc.element.wechat-api.api_custom_service._getRecords)
- description and source-code
```javascript
_getRecords = function (opts, callback) {
  // https://api.weixin.qq.com/customservice/msgrecord/getmsglist?access_token=ACCESS_TOKEN
  opts.msgid = opts.msgid || 1;
  var url = this.endpoint + '/customservice/msgrecord/getmsglist?access_token=' + this.token.accessToken;
  this.request(url, postJSON(opts), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_custom_service._setKfAccountAvatar"></a>[function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>_setKfAccountAvatar (account, filepath, callback)](#apidoc.element.wechat-api.api_custom_service._setKfAccountAvatar)
- description and source-code
```javascript
_setKfAccountAvatar = function (account, filepath, callback) {
  // http://api.weixin.qq.com/customservice/kfaccount/uploadheadimg?access_token=ACCESS_TOKEN&kf_account=KFACCOUNT
  var that = this;
  fs.stat(filepath, function (err, stat) {
    if (err) {
      return callback(err);
    }
    var form = formstream();
    form.file('media', filepath, path.basename(filepath), stat.size);
    var url = this.endpoint + '/customservice/kfaccount/uploadheadimg?access_token=' + that.token.accessToken + '&kf_account=' +
account;
    var opts = {
      dataType: 'json',
      type: 'POST',
      timeout: 60000, // 60秒超时
      headers: form.headers(),
      stream: form
    };
    that.request(url, opts, wrapper(callback));
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_custom_service._updateKfAccount"></a>[function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>_updateKfAccount (account, nick, password, callback)](#apidoc.element.wechat-api.api_custom_service._updateKfAccount)
- description and source-code
```javascript
_updateKfAccount = function (account, nick, password, callback) {
  // https://api.weixin.qq.com/customservice/kfaccount/add?access_token=ACCESS_TOKEN
  var url = this.endpoint + '/customservice/kfaccount/update?access_token=' + this.token.accessToken;
  var data = {
    'kf_account': account,
    'nickname': nick,
    'password': md5(password)
  };

  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_custom_service.addKfAccount"></a>[function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>addKfAccount ()](#apidoc.element.wechat-api.api_custom_service.addKfAccount)
- description and source-code
```javascript
addKfAccount = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...

/**
* 添加客服账号
* 详细请看：http://mp.weixin.qq.com/wiki/9/6fff6f191ef92c126b043ada035cc935.html
*
* Examples:
* '''
* api.addKfAccount('test@test', 'nickname', 'password', callback);
* '''
*
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
...
```

#### <a name="apidoc.element.wechat-api.api_custom_service.deleteKfAccount"></a>[function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>deleteKfAccount ()](#apidoc.element.wechat-api.api_custom_service.deleteKfAccount)
- description and source-code
```javascript
deleteKfAccount = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...

/**
* 删除客服账号
* 详细请看：http://mp.weixin.qq.com/wiki/9/6fff6f191ef92c126b043ada035cc935.html
*
* Examples:
* '''
* api.deleteKfAccount('test@test', callback);
* '''
*
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
...
```

#### <a name="apidoc.element.wechat-api.api_custom_service.getCustomServiceList"></a>[function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>getCustomServiceList ()](#apidoc.element.wechat-api.api_custom_service.getCustomServiceList)
- description and source-code
```javascript
getCustomServiceList = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...

/**
* 获取客服基本信息
* 详细请看：http://dkf.qq.com/document-3_1.html
*
* Examples:
* '''
* api.getCustomServiceList(callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_custom_service.getOnlineCustomServiceList"></a>[function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>getOnlineCustomServiceList ()](#apidoc.element.wechat-api.api_custom_service.getOnlineCustomServiceList)
- description and source-code
```javascript
getOnlineCustomServiceList = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...

/**
* 获取在线客服接待信息
* 详细请看：http://dkf.qq.com/document-3_2.html
*
* Examples:
* '''
* api.getOnlineCustomServiceList(callback);
* '''
*
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
...
```

#### <a name="apidoc.element.wechat-api.api_custom_service.getRecords"></a>[function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>getRecords ()](#apidoc.element.wechat-api.api_custom_service.getRecords)
- description and source-code
```javascript
getRecords = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
*  "endtime" : 987654321,   结束时间，unix时间戳，每次查询时段不能超过24小时
*  "msgid" : 1,             消息id顺序从小到大，从1开始
*  "number" : 10000         每次获取条数，最多10000条
* }
* '''
* Examples:
* '''
* api.getRecords(opts, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_custom_service.setKfAccountAvatar"></a>[function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>setKfAccountAvatar ()](#apidoc.element.wechat-api.api_custom_service.setKfAccountAvatar)
- description and source-code
```javascript
setKfAccountAvatar = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...

/**
* 设置客服头像
* 详细请看：http://mp.weixin.qq.com/wiki/9/6fff6f191ef92c126b043ada035cc935.html
*
* Examples:
* '''
* api.setKfAccountAvatar('test@test', '/path/to/avatar.png', callback);
* '''
*
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
...
```

#### <a name="apidoc.element.wechat-api.api_custom_service.updateKfAccount"></a>[function <span class="apidocSignatureSpan">wechat-api.api_custom_service.</span>updateKfAccount ()](#apidoc.element.wechat-api.api_custom_service.updateKfAccount)
- description and source-code
```javascript
updateKfAccount = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...

/**
* 设置客服账号
* 详细请看：http://mp.weixin.qq.com/wiki/9/6fff6f191ef92c126b043ada035cc935.html
*
* Examples:
* '''
* api.updateKfAccount('test@test', 'nickname', 'password', callback);
* '''
*
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
...
```



# <a name="apidoc.module.wechat-api.api_datacube"></a>[module wechat-api.api_datacube](#apidoc.module.wechat-api.api_datacube)

#### <a name="apidoc.element.wechat-api.api_datacube._getArticleSummary"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getArticleSummary (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getArticleSummary)
- description and source-code
```javascript
_getArticleSummary = function (begin, end, callback) {
  var data = {
    begin_date: begin,
    end_date: end
  };
  var url = this.endpoint + '/datacube/' + method.toLowerCase() + '?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_datacube._getArticleTotal"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getArticleTotal (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getArticleTotal)
- description and source-code
```javascript
_getArticleTotal = function (begin, end, callback) {
  var data = {
    begin_date: begin,
    end_date: end
  };
  var url = this.endpoint + '/datacube/' + method.toLowerCase() + '?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_datacube._getInterfaceSummary"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getInterfaceSummary (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getInterfaceSummary)
- description and source-code
```javascript
_getInterfaceSummary = function (begin, end, callback) {
  var data = {
    begin_date: begin,
    end_date: end
  };
  var url = this.endpoint + '/datacube/' + method.toLowerCase() + '?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_datacube._getInterfaceSummaryHour"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getInterfaceSummaryHour (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getInterfaceSummaryHour)
- description and source-code
```javascript
_getInterfaceSummaryHour = function (begin, end, callback) {
  var data = {
    begin_date: begin,
    end_date: end
  };
  var url = this.endpoint + '/datacube/' + method.toLowerCase() + '?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_datacube._getUpstreamMsg"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getUpstreamMsg (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getUpstreamMsg)
- description and source-code
```javascript
_getUpstreamMsg = function (begin, end, callback) {
  var data = {
    begin_date: begin,
    end_date: end
  };
  var url = this.endpoint + '/datacube/' + method.toLowerCase() + '?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_datacube._getUpstreamMsgDist"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getUpstreamMsgDist (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getUpstreamMsgDist)
- description and source-code
```javascript
_getUpstreamMsgDist = function (begin, end, callback) {
  var data = {
    begin_date: begin,
    end_date: end
  };
  var url = this.endpoint + '/datacube/' + method.toLowerCase() + '?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_datacube._getUpstreamMsgDistMonth"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getUpstreamMsgDistMonth (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getUpstreamMsgDistMonth)
- description and source-code
```javascript
_getUpstreamMsgDistMonth = function (begin, end, callback) {
  var data = {
    begin_date: begin,
    end_date: end
  };
  var url = this.endpoint + '/datacube/' + method.toLowerCase() + '?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_datacube._getUpstreamMsgDistWeek"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getUpstreamMsgDistWeek (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getUpstreamMsgDistWeek)
- description and source-code
```javascript
_getUpstreamMsgDistWeek = function (begin, end, callback) {
  var data = {
    begin_date: begin,
    end_date: end
  };
  var url = this.endpoint + '/datacube/' + method.toLowerCase() + '?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_datacube._getUpstreamMsgHour"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getUpstreamMsgHour (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getUpstreamMsgHour)
- description and source-code
```javascript
_getUpstreamMsgHour = function (begin, end, callback) {
  var data = {
    begin_date: begin,
    end_date: end
  };
  var url = this.endpoint + '/datacube/' + method.toLowerCase() + '?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_datacube._getUpstreamMsgMonth"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getUpstreamMsgMonth (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getUpstreamMsgMonth)
- description and source-code
```javascript
_getUpstreamMsgMonth = function (begin, end, callback) {
  var data = {
    begin_date: begin,
    end_date: end
  };
  var url = this.endpoint + '/datacube/' + method.toLowerCase() + '?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_datacube._getUpstreamMsgWeek"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getUpstreamMsgWeek (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getUpstreamMsgWeek)
- description and source-code
```javascript
_getUpstreamMsgWeek = function (begin, end, callback) {
  var data = {
    begin_date: begin,
    end_date: end
  };
  var url = this.endpoint + '/datacube/' + method.toLowerCase() + '?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_datacube._getUserCumulate"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getUserCumulate (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getUserCumulate)
- description and source-code
```javascript
_getUserCumulate = function (begin, end, callback) {
  var data = {
    begin_date: begin,
    end_date: end
  };
  var url = this.endpoint + '/datacube/' + method.toLowerCase() + '?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_datacube._getUserRead"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getUserRead (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getUserRead)
- description and source-code
```javascript
_getUserRead = function (begin, end, callback) {
  var data = {
    begin_date: begin,
    end_date: end
  };
  var url = this.endpoint + '/datacube/' + method.toLowerCase() + '?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_datacube._getUserReadHour"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getUserReadHour (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getUserReadHour)
- description and source-code
```javascript
_getUserReadHour = function (begin, end, callback) {
  var data = {
    begin_date: begin,
    end_date: end
  };
  var url = this.endpoint + '/datacube/' + method.toLowerCase() + '?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_datacube._getUserShare"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getUserShare (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getUserShare)
- description and source-code
```javascript
_getUserShare = function (begin, end, callback) {
  var data = {
    begin_date: begin,
    end_date: end
  };
  var url = this.endpoint + '/datacube/' + method.toLowerCase() + '?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_datacube._getUserShareHour"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getUserShareHour (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getUserShareHour)
- description and source-code
```javascript
_getUserShareHour = function (begin, end, callback) {
  var data = {
    begin_date: begin,
    end_date: end
  };
  var url = this.endpoint + '/datacube/' + method.toLowerCase() + '?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_datacube._getUserSummary"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>_getUserSummary (begin, end, callback)](#apidoc.element.wechat-api.api_datacube._getUserSummary)
- description and source-code
```javascript
_getUserSummary = function (begin, end, callback) {
  var data = {
    begin_date: begin,
    end_date: end
  };
  var url = this.endpoint + '/datacube/' + method.toLowerCase() + '?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_datacube.getArticleSummary"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getArticleSummary (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getArticleSummary)
- description and source-code
```javascript
getArticleSummary = function (begin, end, callback) {
  this.preRequest(this['_' + method], arguments);
}
```
- example usage
```shell
...
* 详情请见：<http://mp.weixin.qq.com/wiki/8/c0453610fb5131d1fcb17b4e87c82050.html>
* Examples:
* '''
* // 用户分析数据接口
* api.getUserSummary(startDate, endDate, callback); // 获取用户增减数据
* api.getUserCumulate(startDate, endDate, callback); // 获取累计用户数据
* // 图文分析数据接口
* api.getArticleSummary(startDate, endDate, callback); // 获取图文群发每日数据
* api.getArticleTotal(startDate, endDate, callback); // 获取图文群发总数据
* api.getUserRead(startDate, endDate, callback); // 获取图文统计数据
* api.getUserReadHour(startDate, endDate, callback); // 获取图文统计分时数据
* api.getUserShare(startDate, endDate, callback); // 获取图文分享转发数据
* api.getUserShareHour(startDate, endDate, callback); // 获取图文分享转发分时数据
* // 消息分析数据接口
* api.getUpstreamMsg(startDate, endDate, callback); // 获取消息发送概况数据
...
```

#### <a name="apidoc.element.wechat-api.api_datacube.getArticleTotal"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getArticleTotal (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getArticleTotal)
- description and source-code
```javascript
getArticleTotal = function (begin, end, callback) {
  this.preRequest(this['_' + method], arguments);
}
```
- example usage
```shell
...
* Examples:
* '''
* // 用户分析数据接口
* api.getUserSummary(startDate, endDate, callback); // 获取用户增减数据
* api.getUserCumulate(startDate, endDate, callback); // 获取累计用户数据
* // 图文分析数据接口
* api.getArticleSummary(startDate, endDate, callback); // 获取图文群发每日数据
* api.getArticleTotal(startDate, endDate, callback); // 获取图文群发总数据
* api.getUserRead(startDate, endDate, callback); // 获取图文统计数据
* api.getUserReadHour(startDate, endDate, callback); // 获取图文统计分时数据
* api.getUserShare(startDate, endDate, callback); // 获取图文分享转发数据
* api.getUserShareHour(startDate, endDate, callback); // 获取图文分享转发分时数据
* // 消息分析数据接口
* api.getUpstreamMsg(startDate, endDate, callback); // 获取消息发送概况数据
* api.getUpstreamMsgHour(startDate, endDate, callback); // 获取消息分送分时数据
...
```

#### <a name="apidoc.element.wechat-api.api_datacube.getInterfaceSummary"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getInterfaceSummary (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getInterfaceSummary)
- description and source-code
```javascript
getInterfaceSummary = function (begin, end, callback) {
  this.preRequest(this['_' + method], arguments);
}
```
- example usage
```shell
...
* api.getUpstreamMsgHour(startDate, endDate, callback); // 获取消息分送分时数据
* api.getUpstreamMsgWeek(startDate, endDate, callback); // 获取消息发送周数据
* api.getUpstreamMsgMonth(startDate, endDate, callback); // 获取消息发送月数据
* api.getUpstreamMsgDist(startDate, endDate, callback); // 获取消息发送分布数据
* api.getUpstreamMsgDistWeek(startDate, endDate, callback); // 获取消息发送分布周数据
* api.getUpstreamMsgDistMonth(startDate, endDate, callback); // 获取消息发送分布月数据
* // 接口分析数据接口
* api.getInterfaceSummary(startDate, endDate, callback); // 获取接口分析数据
* api.getInterfaceSummaryHour(startDate, endDate, callback); // 获取接口分析分时数据
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
...
```

#### <a name="apidoc.element.wechat-api.api_datacube.getInterfaceSummaryHour"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getInterfaceSummaryHour (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getInterfaceSummaryHour)
- description and source-code
```javascript
getInterfaceSummaryHour = function (begin, end, callback) {
  this.preRequest(this['_' + method], arguments);
}
```
- example usage
```shell
...
* api.getUpstreamMsgWeek(startDate, endDate, callback); // 获取消息发送周数据
* api.getUpstreamMsgMonth(startDate, endDate, callback); // 获取消息发送月数据
* api.getUpstreamMsgDist(startDate, endDate, callback); // 获取消息发送分布数据
* api.getUpstreamMsgDistWeek(startDate, endDate, callback); // 获取消息发送分布周数据
* api.getUpstreamMsgDistMonth(startDate, endDate, callback); // 获取消息发送分布月数据
* // 接口分析数据接口
* api.getInterfaceSummary(startDate, endDate, callback); // 获取接口分析数据
* api.getInterfaceSummaryHour(startDate, endDate, callback); // 获取接口分析分时数据
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_datacube.getUpstreamMsg"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getUpstreamMsg (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getUpstreamMsg)
- description and source-code
```javascript
getUpstreamMsg = function (begin, end, callback) {
  this.preRequest(this['_' + method], arguments);
}
```
- example usage
```shell
...
* api.getArticleSummary(startDate, endDate, callback); // 获取图文群发每日数据
* api.getArticleTotal(startDate, endDate, callback); // 获取图文群发总数据
* api.getUserRead(startDate, endDate, callback); // 获取图文统计数据
* api.getUserReadHour(startDate, endDate, callback); // 获取图文统计分时数据
* api.getUserShare(startDate, endDate, callback); // 获取图文分享转发数据
* api.getUserShareHour(startDate, endDate, callback); // 获取图文分享转发分时数据
* // 消息分析数据接口
* api.getUpstreamMsg(startDate, endDate, callback); // 获取消息发送概况数据
* api.getUpstreamMsgHour(startDate, endDate, callback); // 获取消息分送分时数据
* api.getUpstreamMsgWeek(startDate, endDate, callback); // 获取消息发送周数据
* api.getUpstreamMsgMonth(startDate, endDate, callback); // 获取消息发送月数据
* api.getUpstreamMsgDist(startDate, endDate, callback); // 获取消息发送分布数据
* api.getUpstreamMsgDistWeek(startDate, endDate, callback); // 获取消息发送分布周数据
* api.getUpstreamMsgDistMonth(startDate, endDate, callback); // 获取消息发送分布月数据
* // 接口分析数据接口
...
```

#### <a name="apidoc.element.wechat-api.api_datacube.getUpstreamMsgDist"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getUpstreamMsgDist (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getUpstreamMsgDist)
- description and source-code
```javascript
getUpstreamMsgDist = function (begin, end, callback) {
  this.preRequest(this['_' + method], arguments);
}
```
- example usage
```shell
...
* api.getUserShare(startDate, endDate, callback); // 获取图文分享转发数据
* api.getUserShareHour(startDate, endDate, callback); // 获取图文分享转发分时数据
* // 消息分析数据接口
* api.getUpstreamMsg(startDate, endDate, callback); // 获取消息发送概况数据
* api.getUpstreamMsgHour(startDate, endDate, callback); // 获取消息分送分时数据
* api.getUpstreamMsgWeek(startDate, endDate, callback); // 获取消息发送周数据
* api.getUpstreamMsgMonth(startDate, endDate, callback); // 获取消息发送月数据
* api.getUpstreamMsgDist(startDate, endDate, callback); // 获取消息发送分布数据
* api.getUpstreamMsgDistWeek(startDate, endDate, callback); // 获取消息发送分布周数据
* api.getUpstreamMsgDistMonth(startDate, endDate, callback); // 获取消息发送分布月数据
* // 接口分析数据接口
* api.getInterfaceSummary(startDate, endDate, callback); // 获取接口分析数据
* api.getInterfaceSummaryHour(startDate, endDate, callback); // 获取接口分析分时数据
* '''
* Callback:
...
```

#### <a name="apidoc.element.wechat-api.api_datacube.getUpstreamMsgDistMonth"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getUpstreamMsgDistMonth (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getUpstreamMsgDistMonth)
- description and source-code
```javascript
getUpstreamMsgDistMonth = function (begin, end, callback) {
  this.preRequest(this['_' + method], arguments);
}
```
- example usage
```shell
...
* // 消息分析数据接口
* api.getUpstreamMsg(startDate, endDate, callback); // 获取消息发送概况数据
* api.getUpstreamMsgHour(startDate, endDate, callback); // 获取消息分送分时数据
* api.getUpstreamMsgWeek(startDate, endDate, callback); // 获取消息发送周数据
* api.getUpstreamMsgMonth(startDate, endDate, callback); // 获取消息发送月数据
* api.getUpstreamMsgDist(startDate, endDate, callback); // 获取消息发送分布数据
* api.getUpstreamMsgDistWeek(startDate, endDate, callback); // 获取消息发送分布周数据
* api.getUpstreamMsgDistMonth(startDate, endDate, callback); // 获取消息发送分布月数据
* // 接口分析数据接口
* api.getInterfaceSummary(startDate, endDate, callback); // 获取接口分析数据
* api.getInterfaceSummaryHour(startDate, endDate, callback); // 获取接口分析分时数据
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
...
```

#### <a name="apidoc.element.wechat-api.api_datacube.getUpstreamMsgDistWeek"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getUpstreamMsgDistWeek (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getUpstreamMsgDistWeek)
- description and source-code
```javascript
getUpstreamMsgDistWeek = function (begin, end, callback) {
  this.preRequest(this['_' + method], arguments);
}
```
- example usage
```shell
...
* api.getUserShareHour(startDate, endDate, callback); // 获取图文分享转发分时数据
* // 消息分析数据接口
* api.getUpstreamMsg(startDate, endDate, callback); // 获取消息发送概况数据
* api.getUpstreamMsgHour(startDate, endDate, callback); // 获取消息分送分时数据
* api.getUpstreamMsgWeek(startDate, endDate, callback); // 获取消息发送周数据
* api.getUpstreamMsgMonth(startDate, endDate, callback); // 获取消息发送月数据
* api.getUpstreamMsgDist(startDate, endDate, callback); // 获取消息发送分布数据
* api.getUpstreamMsgDistWeek(startDate, endDate, callback); // 获取消息发送分布周数据
* api.getUpstreamMsgDistMonth(startDate, endDate, callback); // 获取消息发送分布月数据
* // 接口分析数据接口
* api.getInterfaceSummary(startDate, endDate, callback); // 获取接口分析数据
* api.getInterfaceSummaryHour(startDate, endDate, callback); // 获取接口分析分时数据
* '''
* Callback:
*
...
```

#### <a name="apidoc.element.wechat-api.api_datacube.getUpstreamMsgHour"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getUpstreamMsgHour (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getUpstreamMsgHour)
- description and source-code
```javascript
getUpstreamMsgHour = function (begin, end, callback) {
  this.preRequest(this['_' + method], arguments);
}
```
- example usage
```shell
...
* api.getArticleTotal(startDate, endDate, callback); // 获取图文群发总数据
* api.getUserRead(startDate, endDate, callback); // 获取图文统计数据
* api.getUserReadHour(startDate, endDate, callback); // 获取图文统计分时数据
* api.getUserShare(startDate, endDate, callback); // 获取图文分享转发数据
* api.getUserShareHour(startDate, endDate, callback); // 获取图文分享转发分时数据
* // 消息分析数据接口
* api.getUpstreamMsg(startDate, endDate, callback); // 获取消息发送概况数据
* api.getUpstreamMsgHour(startDate, endDate, callback); // 获取消息分送分时数据
* api.getUpstreamMsgWeek(startDate, endDate, callback); // 获取消息发送周数据
* api.getUpstreamMsgMonth(startDate, endDate, callback); // 获取消息发送月数据
* api.getUpstreamMsgDist(startDate, endDate, callback); // 获取消息发送分布数据
* api.getUpstreamMsgDistWeek(startDate, endDate, callback); // 获取消息发送分布周数据
* api.getUpstreamMsgDistMonth(startDate, endDate, callback); // 获取消息发送分布月数据
* // 接口分析数据接口
* api.getInterfaceSummary(startDate, endDate, callback); // 获取接口分析数据
...
```

#### <a name="apidoc.element.wechat-api.api_datacube.getUpstreamMsgMonth"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getUpstreamMsgMonth (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getUpstreamMsgMonth)
- description and source-code
```javascript
getUpstreamMsgMonth = function (begin, end, callback) {
  this.preRequest(this['_' + method], arguments);
}
```
- example usage
```shell
...
* api.getUserReadHour(startDate, endDate, callback); // 获取图文统计分时数据
* api.getUserShare(startDate, endDate, callback); // 获取图文分享转发数据
* api.getUserShareHour(startDate, endDate, callback); // 获取图文分享转发分时数据
* // 消息分析数据接口
* api.getUpstreamMsg(startDate, endDate, callback); // 获取消息发送概况数据
* api.getUpstreamMsgHour(startDate, endDate, callback); // 获取消息分送分时数据
* api.getUpstreamMsgWeek(startDate, endDate, callback); // 获取消息发送周数据
* api.getUpstreamMsgMonth(startDate, endDate, callback); // 获取消息发送月数据
* api.getUpstreamMsgDist(startDate, endDate, callback); // 获取消息发送分布数据
* api.getUpstreamMsgDistWeek(startDate, endDate, callback); // 获取消息发送分布周数据
* api.getUpstreamMsgDistMonth(startDate, endDate, callback); // 获取消息发送分布月数据
* // 接口分析数据接口
* api.getInterfaceSummary(startDate, endDate, callback); // 获取接口分析数据
* api.getInterfaceSummaryHour(startDate, endDate, callback); // 获取接口分析分时数据
* '''
...
```

#### <a name="apidoc.element.wechat-api.api_datacube.getUpstreamMsgWeek"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getUpstreamMsgWeek (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getUpstreamMsgWeek)
- description and source-code
```javascript
getUpstreamMsgWeek = function (begin, end, callback) {
  this.preRequest(this['_' + method], arguments);
}
```
- example usage
```shell
...
* api.getUserRead(startDate, endDate, callback); // 获取图文统计数据
* api.getUserReadHour(startDate, endDate, callback); // 获取图文统计分时数据
* api.getUserShare(startDate, endDate, callback); // 获取图文分享转发数据
* api.getUserShareHour(startDate, endDate, callback); // 获取图文分享转发分时数据
* // 消息分析数据接口
* api.getUpstreamMsg(startDate, endDate, callback); // 获取消息发送概况数据
* api.getUpstreamMsgHour(startDate, endDate, callback); // 获取消息分送分时数据
* api.getUpstreamMsgWeek(startDate, endDate, callback); // 获取消息发送周数据
* api.getUpstreamMsgMonth(startDate, endDate, callback); // 获取消息发送月数据
* api.getUpstreamMsgDist(startDate, endDate, callback); // 获取消息发送分布数据
* api.getUpstreamMsgDistWeek(startDate, endDate, callback); // 获取消息发送分布周数据
* api.getUpstreamMsgDistMonth(startDate, endDate, callback); // 获取消息发送分布月数据
* // 接口分析数据接口
* api.getInterfaceSummary(startDate, endDate, callback); // 获取接口分析数据
* api.getInterfaceSummaryHour(startDate, endDate, callback); // 获取接口分析分时数据
...
```

#### <a name="apidoc.element.wechat-api.api_datacube.getUserCumulate"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getUserCumulate (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getUserCumulate)
- description and source-code
```javascript
getUserCumulate = function (begin, end, callback) {
  this.preRequest(this['_' + method], arguments);
}
```
- example usage
```shell
...
/**
* 公众平台官网数据统计模块
* 详情请见：<http://mp.weixin.qq.com/wiki/8/c0453610fb5131d1fcb17b4e87c82050.html>
* Examples:
* '''
* // 用户分析数据接口
* api.getUserSummary(startDate, endDate, callback); // 获取用户增减数据
* api.getUserCumulate(startDate, endDate, callback); // 获取累计用户数据
* // 图文分析数据接口
* api.getArticleSummary(startDate, endDate, callback); // 获取图文群发每日数据
* api.getArticleTotal(startDate, endDate, callback); // 获取图文群发总数据
* api.getUserRead(startDate, endDate, callback); // 获取图文统计数据
* api.getUserReadHour(startDate, endDate, callback); // 获取图文统计分时数据
* api.getUserShare(startDate, endDate, callback); // 获取图文分享转发数据
* api.getUserShareHour(startDate, endDate, callback); // 获取图文分享转发分时数据
...
```

#### <a name="apidoc.element.wechat-api.api_datacube.getUserRead"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getUserRead (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getUserRead)
- description and source-code
```javascript
getUserRead = function (begin, end, callback) {
  this.preRequest(this['_' + method], arguments);
}
```
- example usage
```shell
...
* '''
* // 用户分析数据接口
* api.getUserSummary(startDate, endDate, callback); // 获取用户增减数据
* api.getUserCumulate(startDate, endDate, callback); // 获取累计用户数据
* // 图文分析数据接口
* api.getArticleSummary(startDate, endDate, callback); // 获取图文群发每日数据
* api.getArticleTotal(startDate, endDate, callback); // 获取图文群发总数据
* api.getUserRead(startDate, endDate, callback); // 获取图文统计数据
* api.getUserReadHour(startDate, endDate, callback); // 获取图文统计分时数据
* api.getUserShare(startDate, endDate, callback); // 获取图文分享转发数据
* api.getUserShareHour(startDate, endDate, callback); // 获取图文分享转发分时数据
* // 消息分析数据接口
* api.getUpstreamMsg(startDate, endDate, callback); // 获取消息发送概况数据
* api.getUpstreamMsgHour(startDate, endDate, callback); // 获取消息分送分时数据
* api.getUpstreamMsgWeek(startDate, endDate, callback); // 获取消息发送周数据
...
```

#### <a name="apidoc.element.wechat-api.api_datacube.getUserReadHour"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getUserReadHour (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getUserReadHour)
- description and source-code
```javascript
getUserReadHour = function (begin, end, callback) {
  this.preRequest(this['_' + method], arguments);
}
```
- example usage
```shell
...
* // 用户分析数据接口
* api.getUserSummary(startDate, endDate, callback); // 获取用户增减数据
* api.getUserCumulate(startDate, endDate, callback); // 获取累计用户数据
* // 图文分析数据接口
* api.getArticleSummary(startDate, endDate, callback); // 获取图文群发每日数据
* api.getArticleTotal(startDate, endDate, callback); // 获取图文群发总数据
* api.getUserRead(startDate, endDate, callback); // 获取图文统计数据
* api.getUserReadHour(startDate, endDate, callback); // 获取图文统计分时数据
* api.getUserShare(startDate, endDate, callback); // 获取图文分享转发数据
* api.getUserShareHour(startDate, endDate, callback); // 获取图文分享转发分时数据
* // 消息分析数据接口
* api.getUpstreamMsg(startDate, endDate, callback); // 获取消息发送概况数据
* api.getUpstreamMsgHour(startDate, endDate, callback); // 获取消息分送分时数据
* api.getUpstreamMsgWeek(startDate, endDate, callback); // 获取消息发送周数据
* api.getUpstreamMsgMonth(startDate, endDate, callback); // 获取消息发送月数据
...
```

#### <a name="apidoc.element.wechat-api.api_datacube.getUserShare"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getUserShare (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getUserShare)
- description and source-code
```javascript
getUserShare = function (begin, end, callback) {
  this.preRequest(this['_' + method], arguments);
}
```
- example usage
```shell
...
* api.getUserSummary(startDate, endDate, callback); // 获取用户增减数据
* api.getUserCumulate(startDate, endDate, callback); // 获取累计用户数据
* // 图文分析数据接口
* api.getArticleSummary(startDate, endDate, callback); // 获取图文群发每日数据
* api.getArticleTotal(startDate, endDate, callback); // 获取图文群发总数据
* api.getUserRead(startDate, endDate, callback); // 获取图文统计数据
* api.getUserReadHour(startDate, endDate, callback); // 获取图文统计分时数据
* api.getUserShare(startDate, endDate, callback); // 获取图文分享转发数据
* api.getUserShareHour(startDate, endDate, callback); // 获取图文分享转发分时数据
* // 消息分析数据接口
* api.getUpstreamMsg(startDate, endDate, callback); // 获取消息发送概况数据
* api.getUpstreamMsgHour(startDate, endDate, callback); // 获取消息分送分时数据
* api.getUpstreamMsgWeek(startDate, endDate, callback); // 获取消息发送周数据
* api.getUpstreamMsgMonth(startDate, endDate, callback); // 获取消息发送月数据
* api.getUpstreamMsgDist(startDate, endDate, callback); // 获取消息发送分布数据
...
```

#### <a name="apidoc.element.wechat-api.api_datacube.getUserShareHour"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getUserShareHour (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getUserShareHour)
- description and source-code
```javascript
getUserShareHour = function (begin, end, callback) {
  this.preRequest(this['_' + method], arguments);
}
```
- example usage
```shell
...
* api.getUserCumulate(startDate, endDate, callback); // 获取累计用户数据
* // 图文分析数据接口
* api.getArticleSummary(startDate, endDate, callback); // 获取图文群发每日数据
* api.getArticleTotal(startDate, endDate, callback); // 获取图文群发总数据
* api.getUserRead(startDate, endDate, callback); // 获取图文统计数据
* api.getUserReadHour(startDate, endDate, callback); // 获取图文统计分时数据
* api.getUserShare(startDate, endDate, callback); // 获取图文分享转发数据
* api.getUserShareHour(startDate, endDate, callback); // 获取图文分享转发分时数据
* // 消息分析数据接口
* api.getUpstreamMsg(startDate, endDate, callback); // 获取消息发送概况数据
* api.getUpstreamMsgHour(startDate, endDate, callback); // 获取消息分送分时数据
* api.getUpstreamMsgWeek(startDate, endDate, callback); // 获取消息发送周数据
* api.getUpstreamMsgMonth(startDate, endDate, callback); // 获取消息发送月数据
* api.getUpstreamMsgDist(startDate, endDate, callback); // 获取消息发送分布数据
* api.getUpstreamMsgDistWeek(startDate, endDate, callback); // 获取消息发送分布周数据
...
```

#### <a name="apidoc.element.wechat-api.api_datacube.getUserSummary"></a>[function <span class="apidocSignatureSpan">wechat-api.api_datacube.</span>getUserSummary (begin, end, callback)](#apidoc.element.wechat-api.api_datacube.getUserSummary)
- description and source-code
```javascript
getUserSummary = function (begin, end, callback) {
  this.preRequest(this['_' + method], arguments);
}
```
- example usage
```shell
...

/**
* 公众平台官网数据统计模块
* 详情请见：<http://mp.weixin.qq.com/wiki/8/c0453610fb5131d1fcb17b4e87c82050.html>
* Examples:
* '''
* // 用户分析数据接口
* api.getUserSummary(startDate, endDate, callback); // 获取用户增减数据
* api.getUserCumulate(startDate, endDate, callback); // 获取累计用户数据
* // 图文分析数据接口
* api.getArticleSummary(startDate, endDate, callback); // 获取图文群发每日数据
* api.getArticleTotal(startDate, endDate, callback); // 获取图文群发总数据
* api.getUserRead(startDate, endDate, callback); // 获取图文统计数据
* api.getUserReadHour(startDate, endDate, callback); // 获取图文统计分时数据
* api.getUserShare(startDate, endDate, callback); // 获取图文分享转发数据
...
```



# <a name="apidoc.module.wechat-api.api_device"></a>[module wechat-api.api_device](#apidoc.module.wechat-api.api_device)

#### <a name="apidoc.element.wechat-api.api_device._authorizeDevices"></a>[function <span class="apidocSignatureSpan">wechat-api.api_device.</span>_authorizeDevices (devices, optype, productid, callback)](#apidoc.element.wechat-api.api_device._authorizeDevices)
- description and source-code
```javascript
_authorizeDevices = function (devices, optype, productid, callback) {
  // https://api.weixin.qq.com/device/authorize_device?access_token=ACCESS_TOKEN
  var url = this.endpoint + '/device/authorize_device?access_token=' + this.token.accessToken;
  var data = {
    'device_num': devices.length,
    'device_list': devices,
    'op_type': optype
  };
  if (typeof productid !== 'function') {
    data.product_id = productid;
  } else {
    callback = productid;
  }
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_device._bindDevice"></a>[function <span class="apidocSignatureSpan">wechat-api.api_device.</span>_bindDevice (deviceId, openid, ticket, callback)](#apidoc.element.wechat-api.api_device._bindDevice)
- description and source-code
```javascript
_bindDevice = function (deviceId, openid, ticket, callback) {
  // https://api.weixin.qq.com/device/bind?access_token=ACCESS_TOKEN
  var url = this.endpoint + '/device/bind?access_token=' + this.token.accessToken;
  var data = {
    ticket: ticket,
    device_id: deviceId,
    openid: openid
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_device._compelBindDevice"></a>[function <span class="apidocSignatureSpan">wechat-api.api_device.</span>_compelBindDevice (deviceId, openid, callback)](#apidoc.element.wechat-api.api_device._compelBindDevice)
- description and source-code
```javascript
_compelBindDevice = function (deviceId, openid, callback) {
  // https://api.weixin.qq.com/device/compel_bind?access_token=ACCESS_TOKEN
  var url = this.endpoint + '/device/compel_bind?access_token=' + this.token.accessToken;
  var data = {
    device_id: deviceId,
    openid: openid
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_device._compelUnbindDevice"></a>[function <span class="apidocSignatureSpan">wechat-api.api_device.</span>_compelUnbindDevice (deviceId, openid, callback)](#apidoc.element.wechat-api.api_device._compelUnbindDevice)
- description and source-code
```javascript
_compelUnbindDevice = function (deviceId, openid, callback) {
  // https://api.weixin.qq.com/device/compel_unbind?access_token=ACCESS_TOKEN
  var url = this.endpoint + '/device/compel_unbind?access_token=' + this.token.accessToken;
  var data = {
    device_id: deviceId,
    openid: openid
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_device._createDeviceQRCode"></a>[function <span class="apidocSignatureSpan">wechat-api.api_device.</span>_createDeviceQRCode (deviceIds, callback)](#apidoc.element.wechat-api.api_device._createDeviceQRCode)
- description and source-code
```javascript
_createDeviceQRCode = function (deviceIds, callback) {
  // https://api.weixin.qq.com/device/create_qrcode?access_token=ACCESS_TOKEN
  var url = this.endpoint + '/device/create_qrcode?access_token=' + this.token.accessToken;
  var info = {
    'device_num': deviceIds.length,
    'device_id_list': deviceIds
  };
  this.request(url, postJSON(info), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_device._getBindDevice"></a>[function <span class="apidocSignatureSpan">wechat-api.api_device.</span>_getBindDevice (openid, callback)](#apidoc.element.wechat-api.api_device._getBindDevice)
- description and source-code
```javascript
_getBindDevice = function (openid, callback) {
  // https://api.weixin.qq.com/device/get_bind_device?access_token=ACCESS_TOKEN&openid=OPENID
  var url = this.endpoint + '/device/get_bind_device?access_token=' + this.token.accessToken + '&openid=' + openid;
  this.request(url, {dataType: 'json'}, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_device._getDeviceQRCode"></a>[function <span class="apidocSignatureSpan">wechat-api.api_device.</span>_getDeviceQRCode (product_id, callback)](#apidoc.element.wechat-api.api_device._getDeviceQRCode)
- description and source-code
```javascript
_getDeviceQRCode = function (product_id, callback) {
  // https://api.weixin.qq.com/device/create_qrcode?access_token=ACCESS_TOKEN
  var url = this.endpoint + '/device/getqrcode?access_token=' + this.token.accessToken + '&product_id=' + product_id;
  this.request(url, {dataType: 'json'}, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_device._getDeviceStatus"></a>[function <span class="apidocSignatureSpan">wechat-api.api_device.</span>_getDeviceStatus (deviceId, callback)](#apidoc.element.wechat-api.api_device._getDeviceStatus)
- description and source-code
```javascript
_getDeviceStatus = function (deviceId, callback) {
  // https://api.weixin.qq.com/device/get_stat?access_token=ACCESS_TOKEN&device_id=DEVICE_ID
  var url = this.endpoint + '/device/get_stat?access_token=' + this.token.accessToken + '&device_id=' + deviceId;
  this.request(url, {dataType: 'json'}, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_device._getOpenID"></a>[function <span class="apidocSignatureSpan">wechat-api.api_device.</span>_getOpenID (deviceId, deviceType, callback)](#apidoc.element.wechat-api.api_device._getOpenID)
- description and source-code
```javascript
_getOpenID = function (deviceId, deviceType, callback) {
  // https://api.weixin.qq.com/device/get_openid?access_token=ACCESS_TOKEN&device_type=DEVICE_TYPE&device_id=DEVICE_ID
  var url = this.endpoint + '/device/get_openid?access_token=' + this.token.accessToken + '&device_id=' + deviceId + '&device_type
=' + deviceType;
  this.request(url, {dataType: 'json'}, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_device._transferMessage"></a>[function <span class="apidocSignatureSpan">wechat-api.api_device.</span>_transferMessage (deviceType, deviceId, openid, content, callback)](#apidoc.element.wechat-api.api_device._transferMessage)
- description and source-code
```javascript
_transferMessage = function (deviceType, deviceId, openid, content, callback) {
  // https://api.weixin.qq.com/device/transmsg?access_token=ACCESS_TOKEN
  var url = this.endpoint + '/device/transmsg?access_token=' + this.token.accessToken;
  var info = {
    'device_type': deviceType,
    'device_id': deviceId,
    'open_id': openid,
    'content': new Buffer(content).toString('base64')
  };
  this.request(url, postJSON(info), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_device._transferStatus"></a>[function <span class="apidocSignatureSpan">wechat-api.api_device.</span>_transferStatus (deviceType, deviceId, openid, status, callback)](#apidoc.element.wechat-api.api_device._transferStatus)
- description and source-code
```javascript
_transferStatus = function (deviceType, deviceId, openid, status, callback) {
  // https://api.weixin.qq.com/device/transmsg?access_token=ACCESS_TOKEN
  var url = this.endpoint + '/device/transmsg?access_token=' + this.token.accessToken;
  var info = {
    'device_type': deviceType,
    'device_id': deviceId,
    'open_id': openid,
    'msg_type': '2',
    'device_status': status
  };
  this.request(url, postJSON(info), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_device._unbindDevice"></a>[function <span class="apidocSignatureSpan">wechat-api.api_device.</span>_unbindDevice (deviceId, openid, ticket, callback)](#apidoc.element.wechat-api.api_device._unbindDevice)
- description and source-code
```javascript
_unbindDevice = function (deviceId, openid, ticket, callback) {
  // https://api.weixin.qq.com/device/unbind?access_token=ACCESS_TOKEN
  var url = this.endpoint + '/device/unbind?access_token=' + this.token.accessToken;
  var data = {
    ticket: ticket,
    device_id: deviceId,
    openid: openid
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_device._verifyDeviceQRCode"></a>[function <span class="apidocSignatureSpan">wechat-api.api_device.</span>_verifyDeviceQRCode (ticket, callback)](#apidoc.element.wechat-api.api_device._verifyDeviceQRCode)
- description and source-code
```javascript
_verifyDeviceQRCode = function (ticket, callback) {
  // https://api.weixin.qq.com/device/verify_qrcode?access_token=ACCESS_TOKEN
  var url = this.endpoint + '/device/verify_qrcode?access_token=' + this.token.accessToken;
  var data = {
    ticket: ticket
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_device.authorizeDevices"></a>[function <span class="apidocSignatureSpan">wechat-api.api_device.</span>authorizeDevices ()](#apidoc.element.wechat-api.api_device.authorizeDevices)
- description and source-code
```javascript
authorizeDevices = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_device.bindDevice"></a>[function <span class="apidocSignatureSpan">wechat-api.api_device.</span>bindDevice ()](#apidoc.element.wechat-api.api_device.bindDevice)
- description and source-code
```javascript
bindDevice = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_device.compelBindDevice"></a>[function <span class="apidocSignatureSpan">wechat-api.api_device.</span>compelBindDevice ()](#apidoc.element.wechat-api.api_device.compelBindDevice)
- description and source-code
```javascript
compelBindDevice = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_device.compelUnbindDevice"></a>[function <span class="apidocSignatureSpan">wechat-api.api_device.</span>compelUnbindDevice ()](#apidoc.element.wechat-api.api_device.compelUnbindDevice)
- description and source-code
```javascript
compelUnbindDevice = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_device.createDeviceQRCode"></a>[function <span class="apidocSignatureSpan">wechat-api.api_device.</span>createDeviceQRCode ()](#apidoc.element.wechat-api.api_device.createDeviceQRCode)
- description and source-code
```javascript
createDeviceQRCode = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_device.getBindDevice"></a>[function <span class="apidocSignatureSpan">wechat-api.api_device.</span>getBindDevice ()](#apidoc.element.wechat-api.api_device.getBindDevice)
- description and source-code
```javascript
getBindDevice = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_device.getDeviceQRCode"></a>[function <span class="apidocSignatureSpan">wechat-api.api_device.</span>getDeviceQRCode ()](#apidoc.element.wechat-api.api_device.getDeviceQRCode)
- description and source-code
```javascript
getDeviceQRCode = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_device.getDeviceStatus"></a>[function <span class="apidocSignatureSpan">wechat-api.api_device.</span>getDeviceStatus ()](#apidoc.element.wechat-api.api_device.getDeviceStatus)
- description and source-code
```javascript
getDeviceStatus = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_device.getOpenID"></a>[function <span class="apidocSignatureSpan">wechat-api.api_device.</span>getOpenID ()](#apidoc.element.wechat-api.api_device.getOpenID)
- description and source-code
```javascript
getOpenID = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_device.transferMessage"></a>[function <span class="apidocSignatureSpan">wechat-api.api_device.</span>transferMessage ()](#apidoc.element.wechat-api.api_device.transferMessage)
- description and source-code
```javascript
transferMessage = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_device.transferStatus"></a>[function <span class="apidocSignatureSpan">wechat-api.api_device.</span>transferStatus ()](#apidoc.element.wechat-api.api_device.transferStatus)
- description and source-code
```javascript
transferStatus = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_device.unbindDevice"></a>[function <span class="apidocSignatureSpan">wechat-api.api_device.</span>unbindDevice ()](#apidoc.element.wechat-api.api_device.unbindDevice)
- description and source-code
```javascript
unbindDevice = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_device.verifyDeviceQRCode"></a>[function <span class="apidocSignatureSpan">wechat-api.api_device.</span>verifyDeviceQRCode ()](#apidoc.element.wechat-api.api_device.verifyDeviceQRCode)
- description and source-code
```javascript
verifyDeviceQRCode = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.wechat-api.api_feedback"></a>[module wechat-api.api_feedback](#apidoc.module.wechat-api.api_feedback)

#### <a name="apidoc.element.wechat-api.api_feedback._updateFeedback"></a>[function <span class="apidocSignatureSpan">wechat-api.api_feedback.</span>_updateFeedback (openid, feedbackId, callback)](#apidoc.element.wechat-api.api_feedback._updateFeedback)
- description and source-code
```javascript
_updateFeedback = function (openid, feedbackId, callback) {
  var feedbackUrl = this.endpoint + '/payfeedback/update';
  // https://api.weixin.qq.com/payfeedback/update?access_token=xxxxx&openid=XXXX&feedbackid=xxxx
  var data = {
    'access_token': this.token.accessToken,
    'openid': openid,
    'feedbackid': feedbackId
  };
  var opts = {
    dataType: 'json',
    type: 'GET',
    data: data,
    headers: {
      'Content-Type': 'application/json'
    }
  };
  this.request(feedbackUrl, opts, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_feedback.updateFeedback"></a>[function <span class="apidocSignatureSpan">wechat-api.api_feedback.</span>updateFeedback (openid, feedbackId, callback)](#apidoc.element.wechat-api.api_feedback.updateFeedback)
- description and source-code
```javascript
updateFeedback = function (openid, feedbackId, callback) {
  this.preRequest(this._updateFeedback, arguments);
}
```
- example usage
```shell
...
var util = require('./util');
var wrapper = util.wrapper;

/**
* 标记客户的投诉处理状态
* Examples:
* '''
* api.updateFeedback(openid, feedbackId, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```



# <a name="apidoc.module.wechat-api.api_group"></a>[module wechat-api.api_group](#apidoc.module.wechat-api.api_group)

#### <a name="apidoc.element.wechat-api.api_group._createGroup"></a>[function <span class="apidocSignatureSpan">wechat-api.api_group.</span>_createGroup (name, callback)](#apidoc.element.wechat-api.api_group._createGroup)
- description and source-code
```javascript
_createGroup = function (name, callback) {
  // https://api.weixin.qq.com/cgi-bin/groups/create?access_token=ACCESS_TOKEN
  // POST数据格式：json
  // POST数据例子：{"group":{"name":"test"}}
  var url = this.endpoint + '/cgi-bin/groups/create?access_token=' + this.token.accessToken;
  var data = {
    'group': {'name': name}
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_group._getGroups"></a>[function <span class="apidocSignatureSpan">wechat-api.api_group.</span>_getGroups (callback)](#apidoc.element.wechat-api.api_group._getGroups)
- description and source-code
```javascript
_getGroups = function (callback) {
  // https://api.weixin.qq.com/cgi-bin/groups/get?access_token=ACCESS_TOKEN
  var url = this.endpoint + '/cgi-bin/groups/get?access_token=' + this.token.accessToken;
  this.request(url, {dataType: 'json'}, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_group._getWhichGroup"></a>[function <span class="apidocSignatureSpan">wechat-api.api_group.</span>_getWhichGroup (openid, callback)](#apidoc.element.wechat-api.api_group._getWhichGroup)
- description and source-code
```javascript
_getWhichGroup = function (openid, callback) {
  // https://api.weixin.qq.com/cgi-bin/groups/getid?access_token=ACCESS_TOKEN
  var url = this.endpoint + '/cgi-bin/groups/getid?access_token=' + this.token.accessToken;
  var data = {
    'openid': openid
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_group._moveUserToGroup"></a>[function <span class="apidocSignatureSpan">wechat-api.api_group.</span>_moveUserToGroup (openid, groupId, callback)](#apidoc.element.wechat-api.api_group._moveUserToGroup)
- description and source-code
```javascript
_moveUserToGroup = function (openid, groupId, callback) {
  // http请求方式: POST（请使用https协议）
  // https://api.weixin.qq.com/cgi-bin/groups/members/update?access_token=ACCESS_TOKEN
  // POST数据格式：json
  // POST数据例子：{"openid":"oDF3iYx0ro3_7jD4HFRDfrjdCM58","to_groupid":108}
  var url = this.endpoint + '/cgi-bin/groups/members/update?access_token=' + this.token.accessToken;
  var data = {
    'openid': openid,
    'to_groupid': groupId
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_group._removeGroup"></a>[function <span class="apidocSignatureSpan">wechat-api.api_group.</span>_removeGroup (groupId, callback)](#apidoc.element.wechat-api.api_group._removeGroup)
- description and source-code
```javascript
_removeGroup = function (groupId, callback) {
  var url = this.endpoint + '/cgi-bin/groups/delete?access_token=' + this.token.accessToken;
  var data = {
    'group': { id: groupId}
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_group._updateGroup"></a>[function <span class="apidocSignatureSpan">wechat-api.api_group.</span>_updateGroup (id, name, callback)](#apidoc.element.wechat-api.api_group._updateGroup)
- description and source-code
```javascript
_updateGroup = function (id, name, callback) {
  // http请求方式: POST（请使用https协议）
  // https://api.weixin.qq.com/cgi-bin/groups/update?access_token=ACCESS_TOKEN
  // POST数据格式：json
  // POST数据例子：{"group":{"id":108,"name":"test2_modify2"}}
  var url = this.endpoint + '/cgi-bin/groups/update?access_token=' + this.token.accessToken;
  var data = {
    'group': {'id': id, 'name': name}
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_group.createGroup"></a>[function <span class="apidocSignatureSpan">wechat-api.api_group.</span>createGroup ()](#apidoc.element.wechat-api.api_group.createGroup)
- description and source-code
```javascript
createGroup = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
});

/**
* 创建分组
* 详情请见：<http://mp.weixin.qq.com/wiki/0/56d992c605a97245eb7e617854b169fc.html>
* Examples:
* '''
* api.createGroup('groupname', callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_group.getGroups"></a>[function <span class="apidocSignatureSpan">wechat-api.api_group.</span>getGroups ()](#apidoc.element.wechat-api.api_group.getGroups)
- description and source-code
```javascript
getGroups = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
var make = util.make;

/**
* 获取分组列表
* 详情请见：<http://mp.weixin.qq.com/wiki/0/56d992c605a97245eb7e617854b169fc.html>
* Examples:
* '''
* api.getGroups(callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_group.getWhichGroup"></a>[function <span class="apidocSignatureSpan">wechat-api.api_group.</span>getWhichGroup ()](#apidoc.element.wechat-api.api_group.getWhichGroup)
- description and source-code
```javascript
getWhichGroup = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
});

/**
* 查询用户在哪个分组
* 详情请见：<http://mp.weixin.qq.com/wiki/0/56d992c605a97245eb7e617854b169fc.html>
* Examples:
* '''
* api.getWhichGroup(openid, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_group.moveUserToGroup"></a>[function <span class="apidocSignatureSpan">wechat-api.api_group.</span>moveUserToGroup ()](#apidoc.element.wechat-api.api_group.moveUserToGroup)
- description and source-code
```javascript
moveUserToGroup = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
});

/**
* 移动用户进分组
* 详情请见：<http://mp.weixin.qq.com/wiki/0/56d992c605a97245eb7e617854b169fc.html>
* Examples:
* '''
* api.moveUserToGroup(openid, groupId, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_group.removeGroup"></a>[function <span class="apidocSignatureSpan">wechat-api.api_group.</span>removeGroup ()](#apidoc.element.wechat-api.api_group.removeGroup)
- description and source-code
```javascript
removeGroup = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
});

/**
* 删除分组
* 详情请见：<http://mp.weixin.qq.com/wiki/0/56d992c605a97245eb7e617854b169fc.html>
* Examples:
* '''
* api.removeGroup(groupId, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_group.updateGroup"></a>[function <span class="apidocSignatureSpan">wechat-api.api_group.</span>updateGroup ()](#apidoc.element.wechat-api.api_group.updateGroup)
- description and source-code
```javascript
updateGroup = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
});

/**
* 更新分组名字
* 详情请见：<http://mp.weixin.qq.com/wiki/0/56d992c605a97245eb7e617854b169fc.html>
* Examples:
* '''
* api.updateGroup(107, 'new groupname', callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```



# <a name="apidoc.module.wechat-api.api_ip"></a>[module wechat-api.api_ip](#apidoc.module.wechat-api.api_ip)

#### <a name="apidoc.element.wechat-api.api_ip._getIp"></a>[function <span class="apidocSignatureSpan">wechat-api.api_ip.</span>_getIp (callback)](#apidoc.element.wechat-api.api_ip._getIp)
- description and source-code
```javascript
_getIp = function (callback) {
  // https://api.weixin.qq.com/cgi-bin/getcallbackip?access_token=ACCESS_TOKEN
  var url = this.endpoint + '/cgi-bin/getcallbackip?access_token=' + this.token.accessToken;
  this.request(url, {dataType: 'json'}, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_ip.getIp"></a>[function <span class="apidocSignatureSpan">wechat-api.api_ip.</span>getIp ()](#apidoc.element.wechat-api.api_ip.getIp)
- description and source-code
```javascript
getIp = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
var make = util.make;

/**
* 获取微信服务器IP地址
* 详情请见：<http://mp.weixin.qq.com/wiki/0/2ad4b6bfd29f30f71d39616c2a0fcedc.html>
* Examples:
* '''
* api.getIp(callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```



# <a name="apidoc.module.wechat-api.api_js"></a>[module wechat-api.api_js](#apidoc.module.wechat-api.api_js)

#### <a name="apidoc.element.wechat-api.api_js._getCardExt"></a>[function <span class="apidocSignatureSpan">wechat-api.api_js.</span>_getCardExt (param, callback)](#apidoc.element.wechat-api.api_js._getCardExt)
- description and source-code
```javascript
_getCardExt = function (param, callback) {
  var apiTicket = this.wxCardTicket.ticket;
  var timestamp = createTimestamp();
  var signature = signCardExt(apiTicket, param.card_id, timestamp, param.code, param.openid, param.balance);
  var result = {
    timestamp: timestamp,
    signature: signature
  };

  result.code = param.code || '';
  result.openid = param.openid || '';

  if (param.balance) {
    result.balance = param.balance;
  }
  callback(null, result);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_js._getJsConfig"></a>[function <span class="apidocSignatureSpan">wechat-api.api_js.</span>_getJsConfig (param, callback)](#apidoc.element.wechat-api.api_js._getJsConfig)
- description and source-code
```javascript
_getJsConfig = function (param, callback) {
  var that = this;
  var nonceStr = createNonceStr();
  var jsAPITicket = this.jsTicket.ticket;
  var timestamp = createTimestamp();
  var signature = sign(nonceStr, jsAPITicket, timestamp, param.url);
  var result = {
    debug: param.debug,
    appId: that.appid,
    timestamp: timestamp,
    nonceStr: nonceStr,
    signature: signature,
    jsApiList: param.jsApiList
  };

  // 判断beta参数是否存在，微信硬件开发用
  // beta: true
  // 开启内测接口调用，注入wx.invoke方法
  if (param.beta) {
    result.beta = param.beta;
  }
  callback(null, result);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_js._getLatestTicket"></a>[function <span class="apidocSignatureSpan">wechat-api.api_js.</span>_getLatestTicket (callback)](#apidoc.element.wechat-api.api_js._getLatestTicket)
- description and source-code
```javascript
_getLatestTicket = function (callback) {
  callback(null, this.jsTicket);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_js._getTicket"></a>[function <span class="apidocSignatureSpan">wechat-api.api_js.</span>_getTicket (type, callback)](#apidoc.element.wechat-api.api_js._getTicket)
- description and source-code
```javascript
_getTicket = function (type, callback) {
  if (typeof type === 'function') {
    callback = type;
    type = 'jsapi';
  }
  var that = this;
  var url = this.endpoint + '/cgi-bin/ticket/getticket?access_token=' + this.token.accessToken + '&type=' + type;
  this.request(url, {dataType: 'json'}, wrapper(function(err, data) {
    if (err) {
      return callback(err);
    }
    // 过期时间，因网络延迟等，将实际过期时间提前10秒，以防止临界点
    var expireTime = (new Date().getTime()) + (data.expires_in - 10) * 1000;
    var ticket = new Ticket(data.ticket, expireTime);
    that.saveTicketToken(type, ticket, function (err) {
      if (err) {
        return callback(err);
      }
      callback(err, ticket);
    });
  }));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_js.getCardExt"></a>[function <span class="apidocSignatureSpan">wechat-api.api_js.</span>getCardExt (param, callback)](#apidoc.element.wechat-api.api_js.getCardExt)
- description and source-code
```javascript
getCardExt = function (param, callback) {
  preRequestWxCardApi.call(this, this._getCardExt, arguments);
}
```
- example usage
```shell
...
* '''
* var param = {
*  card_id: 'p-hXXXXXXX',
*  code: '1234',
*  openid: '111111',
*  balance: 100
* };
* api.getCardExt(param, callback);
* '''
*
* Callback:
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的card_ext对象，包含所需参数
*
* @name getCardExt
...
```

#### <a name="apidoc.element.wechat-api.api_js.getJsConfig"></a>[function <span class="apidocSignatureSpan">wechat-api.api_js.</span>getJsConfig (param, callback)](#apidoc.element.wechat-api.api_js.getJsConfig)
- description and source-code
```javascript
getJsConfig = function (param, callback) {
  preRequestJSApi.call(this, this._getJsConfig, arguments);
}
```
- example usage
```shell
...
* Examples:
* '''
* var param = {
*  debug: false,
*  jsApiList: ['onMenuShareTimeline', 'onMenuShareAppMessage'],
*  url: 'http://www.xxx.com'
* };
* api.getJsConfig(param, callback);
* '''
*
* Callback:
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的js sdk config所需参数
*
* @param {Object} param 参数
...
```

#### <a name="apidoc.element.wechat-api.api_js.getLatestTicket"></a>[function <span class="apidocSignatureSpan">wechat-api.api_js.</span>getLatestTicket (callback)](#apidoc.element.wechat-api.api_js.getLatestTicket)
- description and source-code
```javascript
getLatestTicket = function (callback) {
  preRequestJSApi.call(this, this._getLatestTicket, arguments);
}
```
- example usage
```shell
...
};

/**
* 获取最新的js api ticket
*
* Examples:
* '''
* api.getLatestTicket(callback);
* '''
* Callback:
*
* - 'err', 获取js api ticket出现异常时的异常对象
* - 'ticket', 获取的ticket
*
* @param {Function} callback 回调函数
...
```

#### <a name="apidoc.element.wechat-api.api_js.getTicket"></a>[function <span class="apidocSignatureSpan">wechat-api.api_js.</span>getTicket (type, callback)](#apidoc.element.wechat-api.api_js.getTicket)
- description and source-code
```javascript
getTicket = function (type, callback) {
  this.preRequest(this._getTicket, arguments);
}
```
- example usage
```shell
...
    newargs.push(retryHandle);
    method.apply(that, newargs);
  } else {
    method.apply(that, args);
  }
} else {
  // 从微信端获取ticket
  that.getTicket(function (err, ticket) {
    // 如遇错误，通过回调函数传出
    if (err) {
      return callback(err);
    }
    // 暂时保存ticket
    that.jsTicket = ticket;
    method.apply(that, args);
...
```

#### <a name="apidoc.element.wechat-api.api_js.registerTicketHandle"></a>[function <span class="apidocSignatureSpan">wechat-api.api_js.</span>registerTicketHandle (getTicketToken, saveTicketToken)](#apidoc.element.wechat-api.api_js.registerTicketHandle)
- description and source-code
```javascript
registerTicketHandle = function (getTicketToken, saveTicketToken) {
  if (!getTicketToken && !saveTicketToken) {
    this.ticketStore = {};
  }
  this.getTicketToken = getTicketToken || function (type, callback) {
    if (typeof type === 'function') {
      callback = type;
      type = 'jsapi';
    }
    callback(null, this.ticketStore[type]);
  };

  this.saveTicketToken = saveTicketToken || function (type, ticketToken, callback) {
    // 向下兼容
    if (typeof ticketToken === 'function') {
      callback = ticketToken;
      ticketToken = type;
      type = 'jsapi';
    }

    this.ticketStore[type] = ticketToken;
    if (process.env.NODE_ENV === 'production') {
      console.warn('Dont save ticket in memory, when cluster or multi-computer!');
    }
    callback(null);
  };
}
```
- example usage
```shell
...

/**
* 多台服务器负载均衡时，ticketToken需要外部存储共享。
* 需要调用此registerTicketHandle来设置获取和保存的自定义方法。
*
* Examples:
* '''
* api.registerTicketHandle(getTicketToken, saveTicketToken);
* // getTicketToken
* function getTicketToken(type, callback) {
*  settingModel.getItem(type, {key: 'weixin_ticketToken'}, function (err, setting) {
*    if (err) return callback(err);
*    callback(null, setting.value);
*  });
* }
...
```



# <a name="apidoc.module.wechat-api.api_mass_send"></a>[module wechat-api.api_mass_send](#apidoc.module.wechat-api.api_mass_send)

#### <a name="apidoc.element.wechat-api.api_mass_send._deleteMass"></a>[function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>_deleteMass (messageId, callback)](#apidoc.element.wechat-api.api_mass_send._deleteMass)
- description and source-code
```javascript
_deleteMass = function (messageId, callback) {
  var opts = {
    msg_id: messageId
  };
  var url = this.endpoint + '/cgi-bin/message/mass/delete?access_token=' + this.token.accessToken;
  this.request(url, postJSON(opts), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_mass_send._getMassMessageStatus"></a>[function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>_getMassMessageStatus (messageId, callback)](#apidoc.element.wechat-api.api_mass_send._getMassMessageStatus)
- description and source-code
```javascript
_getMassMessageStatus = function (messageId, callback) {
  var opts = {
    'msg_id': messageId
  };
  var url = this.endpoint + '/cgi-bin/message/mass/get?access_token=' + this.token.accessToken;
  this.request(url, postJSON(opts), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_mass_send._massSend"></a>[function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>_massSend (opts, receivers, callback)](#apidoc.element.wechat-api.api_mass_send._massSend)
- description and source-code
```javascript
_massSend = function (opts, receivers, callback) {
  var url;
  if (Array.isArray(receivers)) {
    opts.touser = receivers;
    url = this.endpoint + '/cgi-bin/message/mass/send?access_token=' + this.token.accessToken;
  } else {
    if (typeof receivers === 'boolean') {
      opts.filter = {
        'is_to_all': receivers
      };
    } else {
      opts.filter = {
        'group_id': receivers
      };
    }
    url = this.endpoint + '/cgi-bin/message/mass/sendall?access_token=' + this.token.accessToken;
  }
  // https://api.weixin.qq.com/cgi-bin/message/mass/sendall?access_token=ACCESS_TOKEN
  this.request(url, postJSON(opts), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_mass_send._previewImage"></a>[function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>_previewImage (openid, mediaId, callback)](#apidoc.element.wechat-api.api_mass_send._previewImage)
- description and source-code
```javascript
_previewImage = function (openid, mediaId, callback) {
  var opts = {
    'touser': openid,
    'image': {
      'media_id': mediaId
    },
    'msgtype': 'image'
  };
  var url = this.endpoint + '/cgi-bin/message/mass/preview?access_token=' + this.token.accessToken;
  this.request(url, postJSON(opts), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_mass_send._previewNews"></a>[function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>_previewNews (openid, mediaId, callback)](#apidoc.element.wechat-api.api_mass_send._previewNews)
- description and source-code
```javascript
_previewNews = function (openid, mediaId, callback) {
  var opts = {
    'touser': openid,
    'mpnews': {
      'media_id': mediaId
    },
    'msgtype': 'mpnews'
  };
  var url = this.endpoint + '/cgi-bin/message/mass/preview?access_token=' + this.token.accessToken;
  this.request(url, postJSON(opts), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_mass_send._previewText"></a>[function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>_previewText (openid, content, callback)](#apidoc.element.wechat-api.api_mass_send._previewText)
- description and source-code
```javascript
_previewText = function (openid, content, callback) {
  var opts = {
    'touser': openid,
    'text': {
      'content': content
    },
    'msgtype':'text'
  };
  var url = this.endpoint + '/cgi-bin/message/mass/preview?access_token=' + this.token.accessToken;
  this.request(url, postJSON(opts), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_mass_send._previewVideo"></a>[function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>_previewVideo (openid, mediaId, callback)](#apidoc.element.wechat-api.api_mass_send._previewVideo)
- description and source-code
```javascript
_previewVideo = function (openid, mediaId, callback) {
  var opts = {
    'touser': openid,
    'mpvideo': {
      'media_id': mediaId
    },
    'msgtype': 'mpvideo'
  };
  var url = this.endpoint + '/cgi-bin/message/mass/preview?access_token=' + this.token.accessToken;
  this.request(url, postJSON(opts), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_mass_send._previewVoice"></a>[function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>_previewVoice (openid, mediaId, callback)](#apidoc.element.wechat-api.api_mass_send._previewVoice)
- description and source-code
```javascript
_previewVoice = function (openid, mediaId, callback) {
  var opts = {
    'touser': openid,
    'voice': {
      'media_id': mediaId
    },
    'msgtype': 'voice'
  };
  var url = this.endpoint + '/cgi-bin/message/mass/preview?access_token=' + this.token.accessToken;
  this.request(url, postJSON(opts), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_mass_send._uploadMPVideo"></a>[function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>_uploadMPVideo (opts, callback)](#apidoc.element.wechat-api.api_mass_send._uploadMPVideo)
- description and source-code
```javascript
_uploadMPVideo = function (opts, callback) {
  // https://file.api.weixin.qq.com/cgi-bin/media/uploadvideo?access_token=ACCESS_TOKEN
  var url = this.fileServerPrefix + 'media/uploadvideo?access_token=' + this.token.accessToken;
  this.request(url, postJSON(opts), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_mass_send._uploadNews"></a>[function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>_uploadNews (news, callback)](#apidoc.element.wechat-api.api_mass_send._uploadNews)
- description and source-code
```javascript
_uploadNews = function (news, callback) {
  // https://api.weixin.qq.com/cgi-bin/media/uploadnews?access_token=ACCESS_TOKEN
  var url = this.endpoint + '/cgi-bin/media/uploadnews?access_token=' + this.token.accessToken;
  this.request(url, postJSON(news), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_mass_send.deleteMass"></a>[function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>deleteMass (messageId, callback)](#apidoc.element.wechat-api.api_mass_send.deleteMass)
- description and source-code
```javascript
deleteMass = function (messageId, callback) {
  this.preRequest(this._deleteMass, arguments);
}
```
- example usage
```shell
...
};

/**
* 删除群发消息
* 详情请见：<http://mp.weixin.qq.com/wiki/15/5380a4e6f02f2ffdc7981a8ed7a40753.html>
* Examples:
* '''
* api.deleteMass(message_id, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_mass_send.getMassMessageStatus"></a>[function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>getMassMessageStatus (messageId, callback)](#apidoc.element.wechat-api.api_mass_send.getMassMessageStatus)
- description and source-code
```javascript
getMassMessageStatus = function (messageId, callback) {
  this.preRequest(this._getMassMessageStatus, arguments);
}
```
- example usage
```shell
...
};

/**
* 查询群发消息状态
* 详情请见：<http://mp.weixin.qq.com/wiki/15/5380a4e6f02f2ffdc7981a8ed7a40753.html>
* Examples:
* '''
* api.getMassMessageStatus(messageId, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_mass_send.massSend"></a>[function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>massSend (opts, receivers, callback)](#apidoc.element.wechat-api.api_mass_send.massSend)
- description and source-code
```javascript
massSend = function (opts, receivers, callback) {
  this.preRequest(this._massSend, arguments);
}
```
- example usage
```shell
...
};

/**
* 群发消息，分别有图文（news）、文本(text)、语音（voice）、图片（image）和视频（video）
* 详情请见：<http://mp.weixin.qq.com/wiki/15/5380a4e6f02f2ffdc7981a8ed7a40753.html>
* Examples:
* '''
* api.massSend(opts, receivers, callback);
* '''
* opts:
* '''
* {
*  "image":{
*    "media_id":"123dsdajkasd231jhksad"
*  },
...
```

#### <a name="apidoc.element.wechat-api.api_mass_send.massSendImage"></a>[function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>massSendImage (mediaId, receivers, callback)](#apidoc.element.wechat-api.api_mass_send.massSendImage)
- description and source-code
```javascript
massSendImage = function (mediaId, receivers, callback) {
  var opts = {
    'image': {
      'media_id': mediaId
    },
    'msgtype': 'image'
  };
  this.massSend(opts, receivers, callback);
}
```
- example usage
```shell
...
};

/**
* 群发图片（image）消息
* 详情请见：<http://mp.weixin.qq.com/wiki/15/5380a4e6f02f2ffdc7981a8ed7a40753.html>
* Examples:
* '''
* api.massSendImage(media_id, receivers, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_mass_send.massSendMPVideo"></a>[function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>massSendMPVideo (data, receivers, callback)](#apidoc.element.wechat-api.api_mass_send.massSendMPVideo)
- description and source-code
```javascript
massSendMPVideo = function (data, receivers, callback) {
  var that = this;
  // 自动帮转视频的media_id
  this.uploadMPVideo(data, function (err, result) {
    if (err) {
      return callback(err);
    }
    that.massSendVideo(result.media_id, receivers, callback);
  });
}
```
- example usage
```shell
...
};

/**
* 群发视频（video）消息，直接通过上传文件得到的media id进行群发（自动生成素材）
* 详情请见：<http://mp.weixin.qq.com/wiki/15/5380a4e6f02f2ffdc7981a8ed7a40753.html>
* Examples:
* '''
* api.massSendMPVideo(data, receivers, callback);
* '''
* Data:
* '''
* {
*  "media_id": "rF4UdIMfYK3efUfyoddYRMU50zMiRmmt_l0kszupYh_SzrcW5Gaheq05p_lHuOTQ",
*  "title": "TITLE",
*  "description": "Description"
...
```

#### <a name="apidoc.element.wechat-api.api_mass_send.massSendNews"></a>[function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>massSendNews (mediaId, receivers, callback)](#apidoc.element.wechat-api.api_mass_send.massSendNews)
- description and source-code
```javascript
massSendNews = function (mediaId, receivers, callback) {
  var opts = {
    'mpnews': {
      'media_id': mediaId
    },
    'msgtype': 'mpnews'
  };
  this.massSend(opts, receivers, callback);
}
```
- example usage
```shell
...
};

/**
* 群发图文（news）消息
* 详情请见：<http://mp.weixin.qq.com/wiki/15/5380a4e6f02f2ffdc7981a8ed7a40753.html>
* Examples:
* '''
* api.massSendNews(mediaId, receivers, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_mass_send.massSendText"></a>[function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>massSendText (content, receivers, callback)](#apidoc.element.wechat-api.api_mass_send.massSendText)
- description and source-code
```javascript
massSendText = function (content, receivers, callback) {
  var opts = {
    'text': {
      'content': content
    },
    'msgtype': 'text'
  };
  this.massSend(opts, receivers, callback);
}
```
- example usage
```shell
...
};

/**
* 群发文字（text）消息
* 详情请见：<http://mp.weixin.qq.com/wiki/15/5380a4e6f02f2ffdc7981a8ed7a40753.html>
* Examples:
* '''
* api.massSendText(content, receivers, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_mass_send.massSendVideo"></a>[function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>massSendVideo (mediaId, receivers, callback)](#apidoc.element.wechat-api.api_mass_send.massSendVideo)
- description and source-code
```javascript
massSendVideo = function (mediaId, receivers, callback) {
  var opts = {
    'mpvideo': {
      'media_id': mediaId
    },
    'msgtype': 'mpvideo'
  };
  this.massSend(opts, receivers, callback);
}
```
- example usage
```shell
...
};

/**
* 群发视频（video）消息
* 详情请见：<http://mp.weixin.qq.com/wiki/15/5380a4e6f02f2ffdc7981a8ed7a40753.html>
* Examples:
* '''
* api.massSendVideo(mediaId, receivers, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_mass_send.massSendVoice"></a>[function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>massSendVoice (mediaId, receivers, callback)](#apidoc.element.wechat-api.api_mass_send.massSendVoice)
- description and source-code
```javascript
massSendVoice = function (mediaId, receivers, callback) {
  var opts = {
    'voice': {
      'media_id': mediaId
    },
    'msgtype': 'voice'
  };
  this.massSend(opts, receivers, callback);
}
```
- example usage
```shell
...
};

/**
* 群发声音（voice）消息
* 详情请见：<http://mp.weixin.qq.com/wiki/15/5380a4e6f02f2ffdc7981a8ed7a40753.html>
* Examples:
* '''
* api.massSendVoice(media_id, receivers, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_mass_send.previewImage"></a>[function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>previewImage (openid, mediaId, callback)](#apidoc.element.wechat-api.api_mass_send.previewImage)
- description and source-code
```javascript
previewImage = function (openid, mediaId, callback) {
  this.preRequest(this._previewImage, arguments);
}
```
- example usage
```shell
...
};

/**
* 预览接口，预览图片消息
* 详情请见：<http://mp.weixin.qq.com/wiki/15/5380a4e6f02f2ffdc7981a8ed7a40753.html>
* Examples:
* '''
* api.previewImage(openid, mediaId, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_mass_send.previewNews"></a>[function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>previewNews (openid, mediaId, callback)](#apidoc.element.wechat-api.api_mass_send.previewNews)
- description and source-code
```javascript
previewNews = function (openid, mediaId, callback) {
  this.preRequest(this._previewNews, arguments);
}
```
- example usage
```shell
...
};

/**
* 预览接口，预览图文消息
* 详情请见：<http://mp.weixin.qq.com/wiki/15/5380a4e6f02f2ffdc7981a8ed7a40753.html>
* Examples:
* '''
* api.previewNews(openid, mediaId, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_mass_send.previewText"></a>[function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>previewText (openid, content, callback)](#apidoc.element.wechat-api.api_mass_send.previewText)
- description and source-code
```javascript
previewText = function (openid, content, callback) {
  this.preRequest(this._previewText, arguments);
}
```
- example usage
```shell
...
};

/**
* 预览接口，预览文本消息
* 详情请见：<http://mp.weixin.qq.com/wiki/15/5380a4e6f02f2ffdc7981a8ed7a40753.html>
* Examples:
* '''
* api.previewText(openid, content, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_mass_send.previewVideo"></a>[function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>previewVideo (openid, mediaId, callback)](#apidoc.element.wechat-api.api_mass_send.previewVideo)
- description and source-code
```javascript
previewVideo = function (openid, mediaId, callback) {
  this.preRequest(this._previewVideo, arguments);
}
```
- example usage
```shell
...
};

/**
* 预览接口，预览视频消息
* 详情请见：<http://mp.weixin.qq.com/wiki/15/5380a4e6f02f2ffdc7981a8ed7a40753.html>
* Examples:
* '''
* api.previewVideo(openid, mediaId, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_mass_send.previewVoice"></a>[function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>previewVoice (openid, mediaId, callback)](#apidoc.element.wechat-api.api_mass_send.previewVoice)
- description and source-code
```javascript
previewVoice = function (openid, mediaId, callback) {
  this.preRequest(this._previewVoice, arguments);
}
```
- example usage
```shell
...
};

/**
* 预览接口，预览语音消息
* 详情请见：<http://mp.weixin.qq.com/wiki/15/5380a4e6f02f2ffdc7981a8ed7a40753.html>
* Examples:
* '''
* api.previewVoice(openid, mediaId, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_mass_send.uploadMPVideo"></a>[function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>uploadMPVideo (opts, callback)](#apidoc.element.wechat-api.api_mass_send.uploadMPVideo)
- description and source-code
```javascript
uploadMPVideo = function (opts, callback) {
  this.preRequest(this._uploadMPVideo, arguments);
}
```
- example usage
```shell
...
};

/**
* 将通过上传下载多媒体文件得到的视频media_id变成视频素材
* 详情请见：<http://mp.weixin.qq.com/wiki/15/5380a4e6f02f2ffdc7981a8ed7a40753.html>
* Examples:
* '''
* api.uploadMPVideo(opts, callback);
* '''
* Opts:
* '''
* {
*  "media_id": "rF4UdIMfYK3efUfyoddYRMU50zMiRmmt_l0kszupYh_SzrcW5Gaheq05p_lHuOTQ",
*  "title": "TITLE",
*  "description": "Description"
...
```

#### <a name="apidoc.element.wechat-api.api_mass_send.uploadNews"></a>[function <span class="apidocSignatureSpan">wechat-api.api_mass_send.</span>uploadNews (news, callback)](#apidoc.element.wechat-api.api_mass_send.uploadNews)
- description and source-code
```javascript
uploadNews = function (news, callback) {
  this.preRequest(this._uploadNews, arguments);
}
```
- example usage
```shell
...
var postJSON = util.postJSON;

/**
* 上传多媒体文件，分别有图片（image）、语音（voice）、视频（video）和缩略图（thumb）
* 详情请见：<http://mp.weixin.qq.com/wiki/15/5380a4e6f02f2ffdc7981a8ed7a40753.html>
* Examples:
* '''
* api.uploadNews(news, callback);
* '''
* News:
* '''
* {
*  "articles": [
*    {
*      "thumb_media_id":"qI6_Ze_6PtV7svjolgs-rN6stStuHIjs9_DidOHaj0Q-mwvBelOXCFZiq2OsIU-p",
...
```



# <a name="apidoc.module.wechat-api.api_material"></a>[module wechat-api.api_material](#apidoc.module.wechat-api.api_material)

#### <a name="apidoc.element.wechat-api.api_material._getMaterial"></a>[function <span class="apidocSignatureSpan">wechat-api.api_material.</span>_getMaterial (mediaId, callback)](#apidoc.element.wechat-api.api_material._getMaterial)
- description and source-code
```javascript
_getMaterial = function (mediaId, callback) {
  var url = this.endpoint + '/cgi-bin/material/get_material?access_token=' + this.token.accessToken;
  var opts = {
    type: 'POST',
    data: {'media_id': mediaId},
    headers: {
      'Content-Type': 'application/json'
    }
  };
  opts.timeout = 60000; // 60秒超时
  this.request(url, opts, wrapper(function (err, data, res) {
    // handle some err
    if (err) {
      return callback(err);
    }
    var contentType = res.headers['content-type'];
    if (contentType === 'application/json') {
      var ret;
      try {
        ret = JSON.parse(data);
        if (ret.errcode) {
          err = new Error(ret.errmsg);
          err.name = 'WeChatAPIError';
        }
      } catch (ex) {
        return callback(ex, data, res);
      }
      return callback(err, ret, res);
    }
    // 输出Buffer对象
    callback(null, data, res);
  }));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_material._getMaterialCount"></a>[function <span class="apidocSignatureSpan">wechat-api.api_material.</span>_getMaterialCount (callback)](#apidoc.element.wechat-api.api_material._getMaterialCount)
- description and source-code
```javascript
_getMaterialCount = function (callback) {
  var url = this.endpoint + '/cgi-bin/material/get_materialcount?access_token=' + this.token.accessToken;
  this.request(url, {dataType: 'json'}, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_material._getMaterials"></a>[function <span class="apidocSignatureSpan">wechat-api.api_material.</span>_getMaterials (type, offset, count, callback)](#apidoc.element.wechat-api.api_material._getMaterials)
- description and source-code
```javascript
_getMaterials = function (type, offset, count, callback) {
  var url = this.endpoint + '/cgi-bin/material/batchget_material?access_token=' + this.token.accessToken;
  var data = {
    type: type,
    offset: offset,
    count: count
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_material._removeMaterial"></a>[function <span class="apidocSignatureSpan">wechat-api.api_material.</span>_removeMaterial (mediaId, callback)](#apidoc.element.wechat-api.api_material._removeMaterial)
- description and source-code
```javascript
_removeMaterial = function (mediaId, callback) {
  var url = this.endpoint + '/cgi-bin/material/del_material?access_token=' + this.token.accessToken;
  this.request(url, postJSON({'media_id': mediaId}), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_material._updateNewsMaterial"></a>[function <span class="apidocSignatureSpan">wechat-api.api_material.</span>_updateNewsMaterial (news, callback)](#apidoc.element.wechat-api.api_material._updateNewsMaterial)
- description and source-code
```javascript
_updateNewsMaterial = function (news, callback) {
  var url = this.endpoint + '/cgi-bin/material/update_news?access_token=' + this.token.accessToken;
  this.request(url, postJSON(news), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_material._uploadMaterial"></a>[function <span class="apidocSignatureSpan">wechat-api.api_material.</span>_uploadMaterial (filepath, type, callback)](#apidoc.element.wechat-api.api_material._uploadMaterial)
- description and source-code
```javascript
_uploadMaterial = function (filepath, type, callback) {
  var that = this;
  fs.stat(filepath, function (err, stat) {
    if (err) {
      return callback(err);
    }
    var form = formstream();
    form.file('media', filepath, path.basename(filepath), stat.size);
    var url = that.endpoint + '/cgi-bin/material/add_material?access_token=' + that.token.accessToken + '&type=' + type;
    var opts = {
      dataType: 'json',
      type: 'POST',
      timeout: 60000, // 60秒超时
      headers: form.headers(),
      stream: form
    };
    that.request(url, opts, wrapper(callback));
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_material._uploadNewsMaterial"></a>[function <span class="apidocSignatureSpan">wechat-api.api_material.</span>_uploadNewsMaterial (news, callback)](#apidoc.element.wechat-api.api_material._uploadNewsMaterial)
- description and source-code
```javascript
_uploadNewsMaterial = function (news, callback) {
  var url = this.endpoint + '/cgi-bin/material/add_news?access_token=' + this.token.accessToken;
  this.request(url, postJSON(news), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_material._uploadVideoMaterial"></a>[function <span class="apidocSignatureSpan">wechat-api.api_material.</span>_uploadVideoMaterial (filepath, description, callback)](#apidoc.element.wechat-api.api_material._uploadVideoMaterial)
- description and source-code
```javascript
_uploadVideoMaterial = function (filepath, description, callback) {
  var that = this;
  fs.stat(filepath, function (err, stat) {
    if (err) {
      return callback(err);
    }
    var form = formstream();
    form.file('media', filepath, path.basename(filepath), stat.size);
    form.field('description', JSON.stringify(description));
    var url = that.endpoint + '/cgi-bin/material/add_material?access_token=' + that.token.accessToken + '&type=video';
    var opts = {
      dataType: 'json',
      type: 'POST',
      timeout: 60000, // 60秒超时
      headers: form.headers(),
      stream: form
    };
    that.request(url, opts, wrapper(callback));
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_material.getMaterial"></a>[function <span class="apidocSignatureSpan">wechat-api.api_material.</span>getMaterial (mediaId, callback)](#apidoc.element.wechat-api.api_material.getMaterial)
- description and source-code
```javascript
getMaterial = function (mediaId, callback) {
  this.preRequest(this._getMaterial, arguments);
}
```
- example usage
```shell
...


/**
* 根据媒体ID获取永久素材
* 详情请见：<http://mp.weixin.qq.com/wiki/4/b3546879f07623cb30df9ca0e420a5d0.html>
* Examples:
* '''
* api.getMaterial('media_id', callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的文件Buffer对象
* - 'res', HTTP响应对象
*
...
```

#### <a name="apidoc.element.wechat-api.api_material.getMaterialCount"></a>[function <span class="apidocSignatureSpan">wechat-api.api_material.</span>getMaterialCount (callback)](#apidoc.element.wechat-api.api_material.getMaterialCount)
- description and source-code
```javascript
getMaterialCount = function (callback) {
  this.preRequest(this._getMaterialCount, arguments);
}
```
- example usage
```shell
...


/**
* 获取素材总数
* 详情请见：<http://mp.weixin.qq.com/wiki/16/8cc64f8c189674b421bee3ed403993b8.html>
* Examples:
* '''
* api.getMaterialCount(callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的文件Buffer对象
* - 'res', HTTP响应对象
*
...
```

#### <a name="apidoc.element.wechat-api.api_material.getMaterials"></a>[function <span class="apidocSignatureSpan">wechat-api.api_material.</span>getMaterials (type, offset, count, callback)](#apidoc.element.wechat-api.api_material.getMaterials)
- description and source-code
```javascript
getMaterials = function (type, offset, count, callback) {
  this.preRequest(this._getMaterials, arguments);
}
```
- example usage
```shell
...
};

/**
* 获取永久素材列表
* 详情请见：<http://mp.weixin.qq.com/wiki/12/2108cd7aafff7f388f41f37efa710204.html>
* Examples:
* '''
* api.getMaterials(type, offset, count, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的文件Buffer对象
* - 'res', HTTP响应对象
*
...
```

#### <a name="apidoc.element.wechat-api.api_material.removeMaterial"></a>[function <span class="apidocSignatureSpan">wechat-api.api_material.</span>removeMaterial (mediaId, callback)](#apidoc.element.wechat-api.api_material.removeMaterial)
- description and source-code
```javascript
removeMaterial = function (mediaId, callback) {
  this.preRequest(this._removeMaterial, arguments);
}
```
- example usage
```shell
...
};

/**
* 删除永久素材
* 详情请见：<http://mp.weixin.qq.com/wiki/5/e66f61c303db51a6c0f90f46b15af5f5.html>
* Examples:
* '''
* api.removeMaterial('media_id', callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的文件Buffer对象
* - 'res', HTTP响应对象
*
...
```

#### <a name="apidoc.element.wechat-api.api_material.updateNewsMaterial"></a>[function <span class="apidocSignatureSpan">wechat-api.api_material.</span>updateNewsMaterial (news, callback)](#apidoc.element.wechat-api.api_material.updateNewsMaterial)
- description and source-code
```javascript
updateNewsMaterial = function (news, callback) {
  this.preRequest(this._updateNewsMaterial, arguments);
}
```
- example usage
```shell
...
*    "content": CONTENT,
*    "content_source_url": CONTENT_SOURCE_URL
*  }
* }
* '''
* Examples:
* '''
* api.updateNewsMaterial(news, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_material.uploadImageMaterial"></a>[function <span class="apidocSignatureSpan">wechat-api.api_material.</span>uploadImageMaterial (filepath, callback)](#apidoc.element.wechat-api.api_material.uploadImageMaterial)
- description and source-code
```javascript
uploadImageMaterial = function (filepath, callback) {
  this.uploadMaterial(filepath, type, callback);
}
```
- example usage
```shell
...
*
* Result:
* '''
* {"type":"TYPE","media_id":"MEDIA_ID","created_at":123456789}
* '''
* Shortcut:
*
* - 'exports.uploadImageMaterial(filepath, callback);'
* - 'exports.uploadVoiceMaterial(filepath, callback);'
* - 'exports.uploadThumbMaterial(filepath, callback);'
*
* @param {String} filepath 文件路径
* @param {String} type 媒体类型，可用值有image、voice、video、thumb
* @param {Function} callback 回调函数
*/
...
```

#### <a name="apidoc.element.wechat-api.api_material.uploadMaterial"></a>[function <span class="apidocSignatureSpan">wechat-api.api_material.</span>uploadMaterial ()](#apidoc.element.wechat-api.api_material.uploadMaterial)
- description and source-code
```javascript
uploadMaterial = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
var make = util.make;

/**
* 上传永久素材，分别有图片（image）、语音（voice）、和缩略图（thumb）
* 详情请见：<http://mp.weixin.qq.com/wiki/14/7e6c03263063f4813141c3e17dd4350a.html>
* Examples:
* '''
* api.uploadMaterial('filepath', type, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_material.uploadNewsMaterial"></a>[function <span class="apidocSignatureSpan">wechat-api.api_material.</span>uploadNewsMaterial (news, callback)](#apidoc.element.wechat-api.api_material.uploadNewsMaterial)
- description and source-code
```javascript
uploadNewsMaterial = function (news, callback) {
  this.preRequest(this._uploadNewsMaterial, arguments);
}
```
- example usage
```shell
...
*    },
*    //若新增的是多图文素材，则此处应还有几段articles结构
*  ]
* }
* '''
* Examples:
* '''
* api.uploadNewsMaterial(news, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_material.uploadThumbMaterial"></a>[function <span class="apidocSignatureSpan">wechat-api.api_material.</span>uploadThumbMaterial (filepath, callback)](#apidoc.element.wechat-api.api_material.uploadThumbMaterial)
- description and source-code
```javascript
uploadThumbMaterial = function (filepath, callback) {
  this.uploadMaterial(filepath, type, callback);
}
```
- example usage
```shell
...
 * '''
 * {"type":"TYPE","media_id":"MEDIA_ID","created_at":123456789}
 * '''
 * Shortcut:
 *
 * - 'exports.uploadImageMaterial(filepath, callback);'
 * - 'exports.uploadVoiceMaterial(filepath, callback);'
 * - 'exports.uploadThumbMaterial(filepath, callback);'
 *
 * @param {String} filepath 文件路径
 * @param {String} type 媒体类型，可用值有image、voice、video、thumb
 * @param {Function} callback 回调函数
 */
make(exports, 'uploadMaterial', function (filepath, type, callback) {
var that = this;
...
```

#### <a name="apidoc.element.wechat-api.api_material.uploadVideoMaterial"></a>[function <span class="apidocSignatureSpan">wechat-api.api_material.</span>uploadVideoMaterial ()](#apidoc.element.wechat-api.api_material.uploadVideoMaterial)
- description and source-code
```javascript
uploadVideoMaterial = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
* 详情请见：<http://mp.weixin.qq.com/wiki/14/7e6c03263063f4813141c3e17dd4350a.html>
* Examples:
* '''
* var description = {
*   "title":VIDEO_TITLE,
*   "introduction":INTRODUCTION
* };
* api.uploadVideoMaterial('filepath', description, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_material.uploadVoiceMaterial"></a>[function <span class="apidocSignatureSpan">wechat-api.api_material.</span>uploadVoiceMaterial (filepath, callback)](#apidoc.element.wechat-api.api_material.uploadVoiceMaterial)
- description and source-code
```javascript
uploadVoiceMaterial = function (filepath, callback) {
  this.uploadMaterial(filepath, type, callback);
}
```
- example usage
```shell
...
 * Result:
 * '''
 * {"type":"TYPE","media_id":"MEDIA_ID","created_at":123456789}
 * '''
 * Shortcut:
 *
 * - 'exports.uploadImageMaterial(filepath, callback);'
 * - 'exports.uploadVoiceMaterial(filepath, callback);'
 * - 'exports.uploadThumbMaterial(filepath, callback);'
 *
 * @param {String} filepath 文件路径
 * @param {String} type 媒体类型，可用值有image、voice、video、thumb
 * @param {Function} callback 回调函数
 */
make(exports, 'uploadMaterial', function (filepath, type, callback) {
...
```



# <a name="apidoc.module.wechat-api.api_media"></a>[module wechat-api.api_media](#apidoc.module.wechat-api.api_media)

#### <a name="apidoc.element.wechat-api.api_media._getMedia"></a>[function <span class="apidocSignatureSpan">wechat-api.api_media.</span>_getMedia (mediaId, callback)](#apidoc.element.wechat-api.api_media._getMedia)
- description and source-code
```javascript
_getMedia = function (mediaId, callback) {
  var url = this.endpoint + '/cgi-bin/media/get?access_token=' + this.token.accessToken + '&media_id=' + mediaId;
  var opts = {
    timeout: 60000 // 60秒超时
  };
  this.request(url, opts, wrapper(function (err, data, res) {
    // handle some err
    if (err) {
      return callback(err);
    }
    var contentType = res.headers['content-type'];
    if (contentType === 'application/json' || contentType === 'text/plain') {
      var ret;
      try {
        ret = JSON.parse(data);
        if (ret.errcode) {
          err = new Error(ret.errmsg);
          err.name = 'WeChatAPIError';
        }
      } catch (ex) {
        callback(ex, data, res);
        return;
      }
      return callback(err, ret, res);
    }
    // 输出Buffer对象
    callback(null, data, res);
  }));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_media._uploadImage"></a>[function <span class="apidocSignatureSpan">wechat-api.api_media.</span>_uploadImage (filepath, callback)](#apidoc.element.wechat-api.api_media._uploadImage)
- description and source-code
```javascript
_uploadImage = function (filepath, callback) {
  var that = this;
  fs.stat(filepath, function (err, stat) {
    if (err) {
      return callback(err);
    }
    var form = formstream();
    form.file('media', filepath, path.basename(filepath), stat.size);
    var url = that.endpoint + '/cgi-bin/media/uploadimg?access_token=' + that.token.accessToken;
    var opts = {
      dataType: 'json',
      type: 'POST',
      timeout: 60000, // 60秒超时
      headers: form.headers(),
      stream: form
    };
    that.request(url, opts, wrapper(callback));
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_media._uploadImageStream"></a>[function <span class="apidocSignatureSpan">wechat-api.api_media.</span>_uploadImageStream (req, callback)](#apidoc.element.wechat-api.api_media._uploadImageStream)
- description and source-code
```javascript
_uploadImageStream = function (req, callback) {
  var that = this;
  var url = that.endpoint + '/cgi-bin/media/uploadimg?access_token=' + that.token.accessToken;
  var opts = {
    dataType: 'json',
    type: 'POST',
    timeout: 60000, // 60秒超时
    headers: req.headers,
    stream: req
  };
  delete opts.headers.host;
  that.request(url, opts, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_media._uploadMedia"></a>[function <span class="apidocSignatureSpan">wechat-api.api_media.</span>_uploadMedia (filepath, type, callback)](#apidoc.element.wechat-api.api_media._uploadMedia)
- description and source-code
```javascript
_uploadMedia = function (filepath, type, callback) {
  var that = this;
  fs.stat(filepath, function (err, stat) {
    if (err) {
      return callback(err);
    }
    var form = formstream();
    form.file('media', filepath, path.basename(filepath), stat.size);
    var url = that.endpoint + '/cgi-bin/media/upload?access_token=' + that.token.accessToken + '&type=' + type;
    var opts = {
      dataType: 'json',
      type: 'POST',
      timeout: 60000, // 60秒超时
      headers: form.headers(),
      stream: form
    };
    that.request(url, opts, wrapper(callback));
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_media.getMedia"></a>[function <span class="apidocSignatureSpan">wechat-api.api_media.</span>getMedia (mediaId, callback)](#apidoc.element.wechat-api.api_media.getMedia)
- description and source-code
```javascript
getMedia = function (mediaId, callback) {
  this.preRequest(this._getMedia, arguments);
}
```
- example usage
```shell
...
});

/**
* 获取临时素材
* 详情请见：<http://mp.weixin.qq.com/wiki/11/07b6b76a6b6e8848e855a435d5e34a5f.html>
* Examples:
* '''
* api.getMedia('media_id', callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的文件Buffer对象
* - 'res', HTTP响应对象
*
...
```

#### <a name="apidoc.element.wechat-api.api_media.uploadImage"></a>[function <span class="apidocSignatureSpan">wechat-api.api_media.</span>uploadImage (filepath, callback)](#apidoc.element.wechat-api.api_media.uploadImage)
- description and source-code
```javascript
uploadImage = function (filepath, callback) {
  this.preRequest(this._uploadImage, arguments);
}
```
- example usage
```shell
...
*
* Result:
* '''
* {"type":"TYPE","media_id":"MEDIA_ID","created_at":123456789}
* '''
* Shortcut:
*
* - 'exports.uploadImage(filepath, callback);'
* - 'exports.uploadVoice(filepath, callback);'
* - 'exports.uploadVideo(filepath, callback);'
* - 'exports.uploadThumb(filepath, callback);'
*
* @param {String} filepath 文件路径
* @param {String} type 媒体类型，可用值有image、voice、video、thumb
* @param {Function} callback 回调函数
...
```

#### <a name="apidoc.element.wechat-api.api_media.uploadImageStream"></a>[function <span class="apidocSignatureSpan">wechat-api.api_media.</span>uploadImageStream (req, callback)](#apidoc.element.wechat-api.api_media.uploadImageStream)
- description and source-code
```javascript
uploadImageStream = function (req, callback) {
  this.preRequest(this._uploadImageStream, arguments);
}
```
- example usage
```shell
...
};

/**
* 上传来自上游管道的图文消息内的图片，并获取URL。
* 拓展于uploadImage，用于客户端直接上传文件管道重定向到微信服务器，不经过自身缓存服务器文件。
* Examples:
* '''
* api.uploadImageStream(req, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_media.uploadMedia"></a>[function <span class="apidocSignatureSpan">wechat-api.api_media.</span>uploadMedia (filepath, type, callback)](#apidoc.element.wechat-api.api_media.uploadMedia)
- description and source-code
```javascript
uploadMedia = function (filepath, type, callback) {
  this.preRequest(this._uploadMedia, arguments);
}
```
- example usage
```shell
...
var wrapper = util.wrapper;

/**
* 新增临时素材，分别有图片（image）、语音（voice）、视频（video）和缩略图（thumb）
* 详情请见：<http://mp.weixin.qq.com/wiki/5/963fc70b80dc75483a271298a76a8d59.html>
* Examples:
* '''
* api.uploadMedia('filepath', type, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_media.uploadThumb"></a>[function <span class="apidocSignatureSpan">wechat-api.api_media.</span>uploadThumb (filepath, callback)](#apidoc.element.wechat-api.api_media.uploadThumb)
- description and source-code
```javascript
uploadThumb = function (filepath, callback) {
  this.uploadMedia(filepath, type, callback);
}
```
- example usage
```shell
...
 * {"type":"TYPE","media_id":"MEDIA_ID","created_at":123456789}
 * '''
 * Shortcut:
 *
 * - 'exports.uploadImage(filepath, callback);'
 * - 'exports.uploadVoice(filepath, callback);'
 * - 'exports.uploadVideo(filepath, callback);'
 * - 'exports.uploadThumb(filepath, callback);'
 *
 * @param {String} filepath 文件路径
 * @param {String} type 媒体类型，可用值有image、voice、video、thumb
 * @param {Function} callback 回调函数
 */
exports.uploadMedia = function (filepath, type, callback) {
this.preRequest(this._uploadMedia, arguments);
...
```

#### <a name="apidoc.element.wechat-api.api_media.uploadVideo"></a>[function <span class="apidocSignatureSpan">wechat-api.api_media.</span>uploadVideo (filepath, callback)](#apidoc.element.wechat-api.api_media.uploadVideo)
- description and source-code
```javascript
uploadVideo = function (filepath, callback) {
  this.uploadMedia(filepath, type, callback);
}
```
- example usage
```shell
...
 * '''
 * {"type":"TYPE","media_id":"MEDIA_ID","created_at":123456789}
 * '''
 * Shortcut:
 *
 * - 'exports.uploadImage(filepath, callback);'
 * - 'exports.uploadVoice(filepath, callback);'
 * - 'exports.uploadVideo(filepath, callback);'
 * - 'exports.uploadThumb(filepath, callback);'
 *
 * @param {String} filepath 文件路径
 * @param {String} type 媒体类型，可用值有image、voice、video、thumb
 * @param {Function} callback 回调函数
 */
exports.uploadMedia = function (filepath, type, callback) {
...
```

#### <a name="apidoc.element.wechat-api.api_media.uploadVoice"></a>[function <span class="apidocSignatureSpan">wechat-api.api_media.</span>uploadVoice (filepath, callback)](#apidoc.element.wechat-api.api_media.uploadVoice)
- description and source-code
```javascript
uploadVoice = function (filepath, callback) {
  this.uploadMedia(filepath, type, callback);
}
```
- example usage
```shell
...
* Result:
* '''
* {"type":"TYPE","media_id":"MEDIA_ID","created_at":123456789}
* '''
* Shortcut:
*
* - 'exports.uploadImage(filepath, callback);'
* - 'exports.uploadVoice(filepath, callback);'
* - 'exports.uploadVideo(filepath, callback);'
* - 'exports.uploadThumb(filepath, callback);'
*
* @param {String} filepath 文件路径
* @param {String} type 媒体类型，可用值有image、voice、video、thumb
* @param {Function} callback 回调函数
*/
...
```



# <a name="apidoc.module.wechat-api.api_menu"></a>[module wechat-api.api_menu](#apidoc.module.wechat-api.api_menu)

#### <a name="apidoc.element.wechat-api.api_menu._createMenu"></a>[function <span class="apidocSignatureSpan">wechat-api.api_menu.</span>_createMenu (menu, callback)](#apidoc.element.wechat-api.api_menu._createMenu)
- description and source-code
```javascript
_createMenu = function (menu, callback) {
  var url = this.endpoint + '/cgi-bin/menu/create?access_token=' + this.token.accessToken;
  this.request(url, postJSON(menu), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_menu._getMenu"></a>[function <span class="apidocSignatureSpan">wechat-api.api_menu.</span>_getMenu (callback)](#apidoc.element.wechat-api.api_menu._getMenu)
- description and source-code
```javascript
_getMenu = function (callback) {
  var url = this.endpoint + '/cgi-bin/menu/get?access_token=' + this.token.accessToken;
  this.request(url, {dataType: 'json'}, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_menu._getMenuConfig"></a>[function <span class="apidocSignatureSpan">wechat-api.api_menu.</span>_getMenuConfig (callback)](#apidoc.element.wechat-api.api_menu._getMenuConfig)
- description and source-code
```javascript
_getMenuConfig = function (callback) {
  var url = this.endpoint + '/cgi-bin/get_current_selfmenu_info?access_token=' + this.token.accessToken;
  this.request(url, {dataType: 'json'}, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_menu._removeMenu"></a>[function <span class="apidocSignatureSpan">wechat-api.api_menu.</span>_removeMenu (callback)](#apidoc.element.wechat-api.api_menu._removeMenu)
- description and source-code
```javascript
_removeMenu = function (callback) {
  var url = this.endpoint + '/cgi-bin/menu/delete?access_token=' + this.token.accessToken;
  this.request(url, {dataType: 'json'}, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_menu.createMenu"></a>[function <span class="apidocSignatureSpan">wechat-api.api_menu.</span>createMenu (menu, callback)](#apidoc.element.wechat-api.api_menu.createMenu)
- description and source-code
```javascript
createMenu = function (menu, callback) {
  this.preRequest(this._createMenu, arguments);
}
```
- example usage
```shell
...
*      }]
*    }
*  ]
* }
* '''
* Examples:
* '''
* api.createMenu(menu, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_menu.getMenu"></a>[function <span class="apidocSignatureSpan">wechat-api.api_menu.</span>getMenu (callback)](#apidoc.element.wechat-api.api_menu.getMenu)
- description and source-code
```javascript
getMenu = function (callback) {
  this.preRequest(this._getMenu, arguments);
}
```
- example usage
```shell
...

/**
* 获取菜单
* 详细请看：<http://mp.weixin.qq.com/wiki/5/f287d1a5b78a35a8884326312ac3e4ed.html>
*
* Examples:
* '''
* api.getMenu(callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result: （注意:如果有个性化菜单被设置,返回的结果会具有更多信息,请参考微信文档)
...
```

#### <a name="apidoc.element.wechat-api.api_menu.getMenuConfig"></a>[function <span class="apidocSignatureSpan">wechat-api.api_menu.</span>getMenuConfig (callback)](#apidoc.element.wechat-api.api_menu.getMenuConfig)
- description and source-code
```javascript
getMenuConfig = function (callback) {
  this.preRequest(this._getMenuConfig, arguments);
}
```
- example usage
```shell
...


/**
* 获取自定义菜单配置
* 详细请看：<http://mp.weixin.qq.com/wiki/17/4dc4b0514fdad7a5fbbd477aa9aab5ed.html>
* Examples:
* '''
* api.getMenuConfig(callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_menu.removeMenu"></a>[function <span class="apidocSignatureSpan">wechat-api.api_menu.</span>removeMenu (callback)](#apidoc.element.wechat-api.api_menu.removeMenu)
- description and source-code
```javascript
removeMenu = function (callback) {
  this.preRequest(this._removeMenu, arguments);
}
```
- example usage
```shell
...
};

/**
* 删除自定义菜单
* 详细请看：<http://mp.weixin.qq.com/wiki/16/8ed41ba931e4845844ad6d1eeb8060c8.html>
* Examples:
* '''
* api.removeMenu(callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```



# <a name="apidoc.module.wechat-api.api_menu_custom"></a>[module wechat-api.api_menu_custom](#apidoc.module.wechat-api.api_menu_custom)

#### <a name="apidoc.element.wechat-api.api_menu_custom._createCustomMenu"></a>[function <span class="apidocSignatureSpan">wechat-api.api_menu_custom.</span>_createCustomMenu (menu, callback)](#apidoc.element.wechat-api.api_menu_custom._createCustomMenu)
- description and source-code
```javascript
_createCustomMenu = function (menu, callback) {
  var url = this.endpoint + '/cgi-bin/menu/addconditional?access_token=' + this.token.accessToken;
  this.request(url, postJSON(menu), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_menu_custom._removeCustomMenu"></a>[function <span class="apidocSignatureSpan">wechat-api.api_menu_custom.</span>_removeCustomMenu (menu_id, callback)](#apidoc.element.wechat-api.api_menu_custom._removeCustomMenu)
- description and source-code
```javascript
_removeCustomMenu = function (menu_id, callback) {
  var url = this.endpoint + '/cgi-bin/menu/delconditional?access_token=' + this.token.accessToken;
  this.request(url, postJSON({
    'menuid' : menu_id
  }), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_menu_custom._testCustomMenu"></a>[function <span class="apidocSignatureSpan">wechat-api.api_menu_custom.</span>_testCustomMenu (user_id, callback)](#apidoc.element.wechat-api.api_menu_custom._testCustomMenu)
- description and source-code
```javascript
_testCustomMenu = function (user_id, callback) {
  var url = this.endpoint + '/cgi-bin/menu/trymatch?access_token=' + this.token.accessToken;
  this.request(url, postJSON({
    'user_id' : user_id
  }), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_menu_custom.createCustomMenu"></a>[function <span class="apidocSignatureSpan">wechat-api.api_menu_custom.</span>createCustomMenu (menu, callback)](#apidoc.element.wechat-api.api_menu_custom.createCustomMenu)
- description and source-code
```javascript
createCustomMenu = function (menu, callback) {
  this.preRequest(this._createCustomMenu, arguments);
}
```
- example usage
```shell
...
*     "city":"广州",
*     "client_platform_type":"2" // IOS(1), Android(2),Others(3)
*   }
* }
* '''
* Examples:
* '''
* api.createCustomMenu(menu, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_menu_custom.removeCustomMenu"></a>[function <span class="apidocSignatureSpan">wechat-api.api_menu_custom.</span>removeCustomMenu (menu_id, callback)](#apidoc.element.wechat-api.api_menu_custom.removeCustomMenu)
- description and source-code
```javascript
removeCustomMenu = function (menu_id, callback) {
  this.preRequest(this._removeCustomMenu, arguments);
}
```
- example usage
```shell
...

/**
* 删除个性化菜单
* 详细请看：<http://mp.weixin.qq.com/wiki/0/c48ccd12b69ae023159b4bfaa7c39c20.html>
*
* Examples:
* '''
* api.removeCustomMenu(menu_id,callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_menu_custom.testCustomMenu"></a>[function <span class="apidocSignatureSpan">wechat-api.api_menu_custom.</span>testCustomMenu (user_id, callback)](#apidoc.element.wechat-api.api_menu_custom.testCustomMenu)
- description and source-code
```javascript
testCustomMenu = function (user_id, callback) {
  this.preRequest(this._testCustomMenu, arguments);
}
```
- example usage
```shell
...

/**
* 测试个性化菜单
* 详细请看：<http://mp.weixin.qq.com/wiki/0/c48ccd12b69ae023159b4bfaa7c39c20.html>
*
* Examples:
* '''
* api.testCustomMenu(user_id,callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```



# <a name="apidoc.module.wechat-api.api_message"></a>[module wechat-api.api_message](#apidoc.module.wechat-api.api_message)

#### <a name="apidoc.element.wechat-api.api_message._sendCard"></a>[function <span class="apidocSignatureSpan">wechat-api.api_message.</span>_sendCard (openid, card, callback)](#apidoc.element.wechat-api.api_message._sendCard)
- description and source-code
```javascript
_sendCard = function (openid, card, callback) {
  var url = this.endpoint + '/cgi-bin/message/custom/send?access_token=' + this.token.accessToken;
  var that = this;
  this.getCardExt(card, function (err, result) {
    var data = {
      'touser': openid,
      'msgtype':'wxcard',
      'wxcard': {
        'card_id': card.card_id,
        'card_ext': result
      }
    };
    that.request(url, postJSON(data), wrapper(callback));
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_message._sendImage"></a>[function <span class="apidocSignatureSpan">wechat-api.api_message.</span>_sendImage (openid, mediaId, callback)](#apidoc.element.wechat-api.api_message._sendImage)
- description and source-code
```javascript
_sendImage = function (openid, mediaId, callback) {
  // {
  //  "touser":"OPENID",
  //  "msgtype":"image",
  //  "image": {
  //    "media_id":"MEDIA_ID"
  //  }
  // }
  var url = this.endpoint + '/cgi-bin/message/custom/send?access_token=' + this.token.accessToken;
  var data = {
    'touser': openid,
    'msgtype':'image',
    'image': {
      'media_id': mediaId
    }
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_message._sendMpNews"></a>[function <span class="apidocSignatureSpan">wechat-api.api_message.</span>_sendMpNews (openid, mediaId, callback)](#apidoc.element.wechat-api.api_message._sendMpNews)
- description and source-code
```javascript
_sendMpNews = function (openid, mediaId, callback) {
   //{
   // "touser":"OPENID",
   // "msgtype":"mpnews",
   // "mpnews":
   //  {
   //     "media_id":"MEDIA_ID"
   //  }
   //}
  var url = this.endpoint + '/cgi-bin/message/custom/send?access_token=' + this.token.accessToken;
  var data = {
    'touser': openid,
    'msgtype':'mpnews',
    'mpnews': {
      'media_id': mediaId
    }
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_message._sendMusic"></a>[function <span class="apidocSignatureSpan">wechat-api.api_message.</span>_sendMusic (openid, music, callback)](#apidoc.element.wechat-api.api_message._sendMusic)
- description and source-code
```javascript
_sendMusic = function (openid, music, callback) {
  // {
  //  "touser":"OPENID",
  //  "msgtype":"music",
  //  "music": {
  //    "title":"MUSIC_TITLE", // 可选
  //    "description":"MUSIC_DESCRIPTION", // 可选
  //    "musicurl":"MUSIC_URL",
  //    "hqmusicurl":"HQ_MUSIC_URL",
  //    "thumb_media_id":"THUMB_MEDIA_ID"
  //  }
  // }
  var url = this.endpoint + '/cgi-bin/message/custom/send?access_token=' + this.token.accessToken;
  var data = {
    'touser': openid,
    'msgtype':'music',
    'music': music
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_message._sendNews"></a>[function <span class="apidocSignatureSpan">wechat-api.api_message.</span>_sendNews (openid, articles, callback)](#apidoc.element.wechat-api.api_message._sendNews)
- description and source-code
```javascript
_sendNews = function (openid, articles, callback) {
  // {
  //  "touser":"OPENID",
  //  "msgtype":"news",
  //  "news":{
  //    "articles": [
  //      {
  //        "title":"Happy Day",
  //        "description":"Is Really A Happy Day",
  //        "url":"URL",
  //        "picurl":"PIC_URL"
  //      },
  //      {
  //        "title":"Happy Day",
  //        "description":"Is Really A Happy Day",
  //        "url":"URL",
  //        "picurl":"PIC_URL"
  //      }]
  //   }
  // }
  var url = this.endpoint + '/cgi-bin/message/custom/send?access_token=' + this.token.accessToken;
  var data = {
    'touser': openid,
    'msgtype':'news',
    'news': {
      'articles': articles
    }
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_message._sendText"></a>[function <span class="apidocSignatureSpan">wechat-api.api_message.</span>_sendText (openid, text, callback)](#apidoc.element.wechat-api.api_message._sendText)
- description and source-code
```javascript
_sendText = function (openid, text, callback) {
  // {
  //  "touser":"OPENID",
  //  "msgtype":"text",
  //  "text": {
  //    "content":"Hello World"
  //  }
  // }
  var url = this.endpoint + '/cgi-bin/message/custom/send?access_token=' + this.token.accessToken;
  var data = {
    'touser': openid,
    'msgtype': 'text',
    'text': {
      'content': text
    }
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_message._sendVideo"></a>[function <span class="apidocSignatureSpan">wechat-api.api_message.</span>_sendVideo (openid, mediaId, thumbMediaId, callback)](#apidoc.element.wechat-api.api_message._sendVideo)
- description and source-code
```javascript
_sendVideo = function (openid, mediaId, thumbMediaId, callback) {
  // {
  //  "touser":"OPENID",
  //  "msgtype":"video",
  //  "video": {
  //    "media_id":"MEDIA_ID"
  //    "thumb_media_id":"THUMB_MEDIA_ID"
  //  }
  // }
  var url = this.endpoint + '/cgi-bin/message/custom/send?access_token=' + this.token.accessToken;
  var data = {
    'touser': openid,
    'msgtype':'video',
    'video': {
      'media_id': mediaId,
      'thumb_media_id': thumbMediaId
    }
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_message._sendVoice"></a>[function <span class="apidocSignatureSpan">wechat-api.api_message.</span>_sendVoice (openid, mediaId, callback)](#apidoc.element.wechat-api.api_message._sendVoice)
- description and source-code
```javascript
_sendVoice = function (openid, mediaId, callback) {
  // {
  //  "touser":"OPENID",
  //  "msgtype":"voice",
  //  "voice": {
  //    "media_id":"MEDIA_ID"
  //  }
  // }
  var url = this.endpoint + '/cgi-bin/message/custom/send?access_token=' + this.token.accessToken;
  var data = {
    'touser': openid,
    'msgtype': 'voice',
    'voice': {
      'media_id': mediaId
    }
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_message.sendCard"></a>[function <span class="apidocSignatureSpan">wechat-api.api_message.</span>sendCard (openid, card, callback)](#apidoc.element.wechat-api.api_message.sendCard)
- description and source-code
```javascript
sendCard = function (openid, card, callback) {
  this.preRequest(this._sendCard, arguments);
}
```
- example usage
```shell
...
};

/**
* 客服消息，发送卡卷消息
* 详细细节 http://mp.weixin.qq.com/wiki/1/70a29afed17f56d537c833f89be979c9.html#.E5.AE.A2.E6.9C.8D.E6.8E.A5.E5.8F.A3-.E5.8F.91.E6.B6
.88.E6.81.AF
* Examples:
* '''
* api.sendCard('openid', 'card', callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* @param {String} openid 用户的openid
...
```

#### <a name="apidoc.element.wechat-api.api_message.sendImage"></a>[function <span class="apidocSignatureSpan">wechat-api.api_message.</span>sendImage (openid, mediaId, callback)](#apidoc.element.wechat-api.api_message.sendImage)
- description and source-code
```javascript
sendImage = function (openid, mediaId, callback) {
  this.preRequest(this._sendImage, arguments);
}
```
- example usage
```shell
...
};

/**
* 客服消息，发送图片消息
* 详细细节 http://mp.weixin.qq.com/wiki/1/70a29afed17f56d537c833f89be979c9.html#.E5.AE.A2.E6.9C.8D.E6.8E.A5.E5.8F.A3-.E5.8F.91.E6.B6
.88.E6.81.AF
* Examples:
* '''
* api.sendImage('openid', 'media_id', callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* @param {String} openid 用户的openid
...
```

#### <a name="apidoc.element.wechat-api.api_message.sendMpNews"></a>[function <span class="apidocSignatureSpan">wechat-api.api_message.</span>sendMpNews (openid, mediaId, callback)](#apidoc.element.wechat-api.api_message.sendMpNews)
- description and source-code
```javascript
sendMpNews = function (openid, mediaId, callback) {
  this.preRequest(this._sendMpNews, arguments);
}
```
- example usage
```shell
...


/**
* 客服消息，发送图文消息（点击跳转到图文消息页面）
* 详细细节 http://mp.weixin.qq.com/wiki/14/d9be34fe03412c92517da10a5980e7ee.html#.E5.AE.A2.E6.9C.8D.E6.8E.A5.E5.8F.A3-.E5.8F.91.E6.B6
.88.E6.81.AF
* Examples:
* '''
* api.sendMpNews('openid', 'mediaId' , callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* @param {String} openid 用户的openid
...
```

#### <a name="apidoc.element.wechat-api.api_message.sendMusic"></a>[function <span class="apidocSignatureSpan">wechat-api.api_message.</span>sendMusic (openid, music, callback)](#apidoc.element.wechat-api.api_message.sendMusic)
- description and source-code
```javascript
sendMusic = function (openid, music, callback) {
  this.preRequest(this._sendMusic, arguments);
}
```
- example usage
```shell
...
* var music = {
*  title: '音乐标题', // 可选
*  description: '描述内容', // 可选
*  musicurl: 'http://url.cn/xxx', 音乐文件地址
*  hqmusicurl: "HQ_MUSIC_URL",
*  thumb_media_id: "THUMB_MEDIA_ID"
* };
* api.sendMusic('openid', music, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* @param {String} openid 用户的openid
...
```

#### <a name="apidoc.element.wechat-api.api_message.sendNews"></a>[function <span class="apidocSignatureSpan">wechat-api.api_message.</span>sendNews (openid, articles, callback)](#apidoc.element.wechat-api.api_message.sendNews)
- description and source-code
```javascript
sendNews = function (openid, articles, callback) {
  this.preRequest(this._sendNews, arguments);
}
```
- example usage
```shell
...
*  },
*  {
*    "title":"Happy Day",
*    "description":"Is Really A Happy Day",
*    "url":"URL",
*    "picurl":"PIC_URL"
*  }];
* api.sendNews('openid', articles, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* @param {String} openid 用户的openid
...
```

#### <a name="apidoc.element.wechat-api.api_message.sendText"></a>[function <span class="apidocSignatureSpan">wechat-api.api_message.</span>sendText (openid, text, callback)](#apidoc.element.wechat-api.api_message.sendText)
- description and source-code
```javascript
sendText = function (openid, text, callback) {
  this.preRequest(this._sendText, arguments);
}
```
- example usage
```shell
...
var postJSON = util.postJSON;

/**
* 客服消息，发送文字消息
* 详细细节 http://mp.weixin.qq.com/wiki/1/70a29afed17f56d537c833f89be979c9.html#.E5.AE.A2.E6.9C.8D.E6.8E.A5.E5.8F.A3-.E5.8F.91.E6.B6
.88.E6.81.AF
* Examples:
* '''
* api.sendText('openid', 'Hello world', callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* @param {String} openid 用户的openid
...
```

#### <a name="apidoc.element.wechat-api.api_message.sendVideo"></a>[function <span class="apidocSignatureSpan">wechat-api.api_message.</span>sendVideo (openid, mediaId, thumbMediaId, callback)](#apidoc.element.wechat-api.api_message.sendVideo)
- description and source-code
```javascript
sendVideo = function (openid, mediaId, thumbMediaId, callback) {
  this.preRequest(this._sendVideo, arguments);
}
```
- example usage
```shell
...
};

/**
* 客服消息，发送视频消息
* 详细细节 http://mp.weixin.qq.com/wiki/1/70a29afed17f56d537c833f89be979c9.html#.E5.AE.A2.E6.9C.8D.E6.8E.A5.E5.8F.A3-.E5.8F.91.E6.B6
.88.E6.81.AF
* Examples:
* '''
* api.sendVideo('openid', 'media_id', 'thumb_media_id', callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* @param {String} openid 用户的openid
...
```

#### <a name="apidoc.element.wechat-api.api_message.sendVoice"></a>[function <span class="apidocSignatureSpan">wechat-api.api_message.</span>sendVoice (openid, mediaId, callback)](#apidoc.element.wechat-api.api_message.sendVoice)
- description and source-code
```javascript
sendVoice = function (openid, mediaId, callback) {
  this.preRequest(this._sendVoice, arguments);
}
```
- example usage
```shell
...
};

/**
* 客服消息，发送语音消息
* 详细细节 http://mp.weixin.qq.com/wiki/1/70a29afed17f56d537c833f89be979c9.html#.E5.AE.A2.E6.9C.8D.E6.8E.A5.E5.8F.A3-.E5.8F.91.E6.B6
.88.E6.81.AF
* Examples:
* '''
* api.sendVoice('openid', 'media_id', callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* @param {String} openid 用户的openid
...
```



# <a name="apidoc.module.wechat-api.api_payment"></a>[module wechat-api.api_payment](#apidoc.module.wechat-api.api_payment)

#### <a name="apidoc.element.wechat-api.api_payment._deliverNotify"></a>[function <span class="apidocSignatureSpan">wechat-api.api_payment.</span>_deliverNotify (data, callback)](#apidoc.element.wechat-api.api_payment._deliverNotify)
- description and source-code
```javascript
_deliverNotify = function (data, callback) {
  var url = this.endpoint + '/pay/delivernotify?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_payment._orderQuery"></a>[function <span class="apidocSignatureSpan">wechat-api.api_payment.</span>_orderQuery (query, callback)](#apidoc.element.wechat-api.api_payment._orderQuery)
- description and source-code
```javascript
_orderQuery = function (query, callback) {
  var url = this.endpoint + '/pay/orderquery?access_token=' + this.token.accessToken;
  this.request(url, postJSON(query), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_payment.deliverNotify"></a>[function <span class="apidocSignatureSpan">wechat-api.api_payment.</span>deliverNotify (data, callback)](#apidoc.element.wechat-api.api_payment.deliverNotify)
- description and source-code
```javascript
deliverNotify = function (data, callback) {
  this.preRequest(this._deliverNotify, arguments);
}
```
- example usage
```shell
...
*   "deliver_msg" : "ok",
*   "app_signature" : "53cca9d47b883bd4a5c85a9300df3da0cb48565c",
*   "sign_method" : "sha1"
* }
* '''
* Examples:
* '''
* api.deliverNotify(data, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_payment.orderQuery"></a>[function <span class="apidocSignatureSpan">wechat-api.api_payment.</span>orderQuery (query, callback)](#apidoc.element.wechat-api.api_payment.orderQuery)
- description and source-code
```javascript
orderQuery = function (query, callback) {
  this.preRequest(this._orderQuery, arguments);
}
```
- example usage
```shell
...
*   "timestamp" : "1369745073",
*   "app_signature" : "53cca9d47b883bd4a5c85a9300df3da0cb48565c",
*   "sign_method" : "sha1"
* }
* '''
* Examples:
* '''
* api.orderQuery(query, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```



# <a name="apidoc.module.wechat-api.api_poi"></a>[module wechat-api.api_poi](#apidoc.module.wechat-api.api_poi)

#### <a name="apidoc.element.wechat-api.api_poi._addPoi"></a>[function <span class="apidocSignatureSpan">wechat-api.api_poi.</span>_addPoi (poi, callback)](#apidoc.element.wechat-api.api_poi._addPoi)
- description and source-code
```javascript
_addPoi = function (poi, callback) {
  var data = {
    business: {
      base_info: poi
    }
  };
  var url = this.endpoint + '/cgi-bin/poi/addpoi?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_poi._delPoi"></a>[function <span class="apidocSignatureSpan">wechat-api.api_poi.</span>_delPoi (poiId, callback)](#apidoc.element.wechat-api.api_poi._delPoi)
- description and source-code
```javascript
_delPoi = function (poiId, callback) {
  var url = this.endpoint + '/cgi-bin/poi/delpoi?access_token=' + this.token.accessToken;
  var data = {
    poi_id: poiId
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_poi._getPoi"></a>[function <span class="apidocSignatureSpan">wechat-api.api_poi.</span>_getPoi (poiId, callback)](#apidoc.element.wechat-api.api_poi._getPoi)
- description and source-code
```javascript
_getPoi = function (poiId, callback) {
  var url = this.endpoint + '/cgi-bin/poi/getpoi?access_token=' + this.token.accessToken;
  var data = {
    poi_id: poiId
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_poi._getPois"></a>[function <span class="apidocSignatureSpan">wechat-api.api_poi.</span>_getPois (begin, limit, callback)](#apidoc.element.wechat-api.api_poi._getPois)
- description and source-code
```javascript
_getPois = function (begin, limit, callback) {
  var url = this.endpoint + '/cgi-bin/poi/getpoilist?access_token=' + this.token.accessToken;
  var data = {
    begin: begin,
    limit: limit
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_poi._getWXCategory"></a>[function <span class="apidocSignatureSpan">wechat-api.api_poi.</span>_getWXCategory (callback)](#apidoc.element.wechat-api.api_poi._getWXCategory)
- description and source-code
```javascript
_getWXCategory = function (callback) {
  var url = this.endpoint + '/cgi-bin/poi/getwxcategory?access_token=' + this.token.accessToken;
  this.request(url, {dataType: 'json'}, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_poi._updatePoi"></a>[function <span class="apidocSignatureSpan">wechat-api.api_poi.</span>_updatePoi (poi, callback)](#apidoc.element.wechat-api.api_poi._updatePoi)
- description and source-code
```javascript
_updatePoi = function (poi, callback) {
  var data = {
    business: {
      base_info: poi
    }
  };
  var url = this.endpoint + '/cgi-bin/poi/updatepoi?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_poi.addPoi"></a>[function <span class="apidocSignatureSpan">wechat-api.api_poi.</span>addPoi ()](#apidoc.element.wechat-api.api_poi.addPoi)
- description and source-code
```javascript
addPoi = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
*   "introduction": "肯打鸡是全球大型跨国连锁餐厅,2015年创立于米国,在世界上大约拥有3 亿间分店,主要售卖肯打鸡等垃圾食品",
*   "open_time": "10:00-18:00",
*   "avg_price": 88
* }
* '''
* Examples:
* '''
* api.addPoi(poi, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_poi.delPoi"></a>[function <span class="apidocSignatureSpan">wechat-api.api_poi.</span>delPoi ()](#apidoc.element.wechat-api.api_poi.delPoi)
- description and source-code
```javascript
delPoi = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
*
* Tips:
*
* - 待审核门店不允许删除
*
* Examples:
* '''
* api.delPoi(POI_ID, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* @name delPoi
...
```

#### <a name="apidoc.element.wechat-api.api_poi.getPoi"></a>[function <span class="apidocSignatureSpan">wechat-api.api_poi.</span>getPoi ()](#apidoc.element.wechat-api.api_poi.getPoi)
- description and source-code
```javascript
getPoi = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
});

/**
* 获取门店信息
*
* Examples:
* '''
* api.getPoi(POI_ID, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_poi.getPois"></a>[function <span class="apidocSignatureSpan">wechat-api.api_poi.</span>getPois ()](#apidoc.element.wechat-api.api_poi.getPois)
- description and source-code
```javascript
getPois = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
 this.request(url, postJSON(data), wrapper(callback));
});

/**
* 获取门店列表
* Examples:
* '''
* api.getPois(0, 20, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_poi.getWXCategory"></a>[function <span class="apidocSignatureSpan">wechat-api.api_poi.</span>getWXCategory ()](#apidoc.element.wechat-api.api_poi.getWXCategory)
- description and source-code
```javascript
getWXCategory = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
*
* Tips:
*
* - 类目名称接口是为商户提供自己门店类型信息的接口。门店类目定位的越规范，能够精准的吸引更多用户，提高曝光率。
*
* Examples:
* '''
* api.getWXCategory(callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* @name getWXCategory
...
```

#### <a name="apidoc.element.wechat-api.api_poi.updatePoi"></a>[function <span class="apidocSignatureSpan">wechat-api.api_poi.</span>updatePoi ()](#apidoc.element.wechat-api.api_poi.updatePoi)
- description and source-code
```javascript
updatePoi = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
* }
* '''
* 特别注意，以上7个字段，若有填写内容则为覆盖更新，若无内容则视为不修改，维持原有内容。
* photo_list字段为全列表覆盖，若需要增加图片，需将之前图片同样放入list中，在其后增加新增图片。
*
* Examples:
* '''
* api.updatePoi(poi, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```



# <a name="apidoc.module.wechat-api.api_qrcode"></a>[module wechat-api.api_qrcode](#apidoc.module.wechat-api.api_qrcode)

#### <a name="apidoc.element.wechat-api.api_qrcode._createLimitQRCode"></a>[function <span class="apidocSignatureSpan">wechat-api.api_qrcode.</span>_createLimitQRCode (sceneId, callback)](#apidoc.element.wechat-api.api_qrcode._createLimitQRCode)
- description and source-code
```javascript
_createLimitQRCode = function (sceneId, callback) {
  var url = this.endpoint + '/cgi-bin/qrcode/create?access_token=' + this.token.accessToken;
  var data = {
    'action_name': 'QR_LIMIT_SCENE',
    'action_info': {'scene': {'scene_id': sceneId}}
  };
  // 字符串
  if (typeof sceneId === 'string') {
    data.action_name = 'QR_LIMIT_STR_SCENE';
    data.action_info.scene = {'scene_str': sceneId};
  }
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_qrcode._createTmpQRCode"></a>[function <span class="apidocSignatureSpan">wechat-api.api_qrcode.</span>_createTmpQRCode (sceneId, expire, callback)](#apidoc.element.wechat-api.api_qrcode._createTmpQRCode)
- description and source-code
```javascript
_createTmpQRCode = function (sceneId, expire, callback) {
  var url = this.endpoint + '/cgi-bin/qrcode/create?access_token=' + this.token.accessToken;
  var data = {
    'expire_seconds': expire,
    'action_name': 'QR_SCENE',
    'action_info': {'scene': {'scene_id': sceneId}}
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_qrcode.createLimitQRCode"></a>[function <span class="apidocSignatureSpan">wechat-api.api_qrcode.</span>createLimitQRCode (sceneId, callback)](#apidoc.element.wechat-api.api_qrcode.createLimitQRCode)
- description and source-code
```javascript
createLimitQRCode = function (sceneId, callback) {
  this.preRequest(this._createLimitQRCode, arguments);
}
```
- example usage
```shell
...
};

/**
* 创建永久二维码
* 详细请看：<http://mp.weixin.qq.com/wiki/18/28fc21e7ed87bec960651f0ce873ef8a.html>
* Examples:
* '''
* api.createLimitQRCode(100, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_qrcode.createTmpQRCode"></a>[function <span class="apidocSignatureSpan">wechat-api.api_qrcode.</span>createTmpQRCode (sceneId, expire, callback)](#apidoc.element.wechat-api.api_qrcode.createTmpQRCode)
- description and source-code
```javascript
createTmpQRCode = function (sceneId, expire, callback) {
  this.preRequest(this._createTmpQRCode, arguments);
}
```
- example usage
```shell
...
var postJSON = util.postJSON;

/**
* 创建临时二维码
* 详细请看：<http://mp.weixin.qq.com/wiki/18/28fc21e7ed87bec960651f0ce873ef8a.html>
* Examples:
* '''
* api.createTmpQRCode(10000, 1800, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_qrcode.showQRCodeURL"></a>[function <span class="apidocSignatureSpan">wechat-api.api_qrcode.</span>showQRCodeURL (ticket)](#apidoc.element.wechat-api.api_qrcode.showQRCodeURL)
- description and source-code
```javascript
showQRCodeURL = function (ticket) {
  return this.mpPrefix + 'showqrcode?ticket=' + ticket;
}
```
- example usage
```shell
...
this.request(url, postJSON(data), wrapper(callback));
};

/**
 * 生成显示二维码的链接。微信扫描后，可立即进入场景
 * Examples:
 * '''
 * api.showQRCodeURL(titck);
 * // => https://mp.weixin.qq.com/cgi-bin/showqrcode?ticket=TICKET
 * '''
 * @param {String} ticket 二维码Ticket
 * @return {String} 显示二维码的URL地址，通过img标签可以显示出来
 */
exports.showQRCodeURL = function (ticket) {
return this.mpPrefix + 'showqrcode?ticket=' + ticket;
...
```



# <a name="apidoc.module.wechat-api.api_quota"></a>[module wechat-api.api_quota](#apidoc.module.wechat-api.api_quota)

#### <a name="apidoc.element.wechat-api.api_quota._clearQuota"></a>[function <span class="apidocSignatureSpan">wechat-api.api_quota.</span>_clearQuota (appid, callback)](#apidoc.element.wechat-api.api_quota._clearQuota)
- description and source-code
```javascript
_clearQuota = function (appid, callback) {
  var data = {
    appid: appid
  };
  // https://api.weixin.qq.com/cgi-bin/clear_quota?access_token=ACCESS_TOKEN
  var url = this.endpoint + '/cgi-bin/clear_quota?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_quota.clearQuota"></a>[function <span class="apidocSignatureSpan">wechat-api.api_quota.</span>clearQuota ()](#apidoc.element.wechat-api.api_quota.clearQuota)
- description and source-code
```javascript
clearQuota = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.wechat-api.api_semantic"></a>[module wechat-api.api_semantic](#apidoc.module.wechat-api.api_semantic)

#### <a name="apidoc.element.wechat-api.api_semantic._semantic"></a>[function <span class="apidocSignatureSpan">wechat-api.api_semantic.</span>_semantic (uid, opts, callback)](#apidoc.element.wechat-api.api_semantic._semantic)
- description and source-code
```javascript
_semantic = function (uid, opts, callback) {
  // https://api.weixin.qq.com/semantic/semproxy/search?access_token=YOUR_ACCESS_TOKEN
  var url = this.endpoint + '/semantic/semproxy/search?access_token=' + this.token.accessToken;
  opts.appid = this.appid;
  opts.uid = uid;
  this.request(url, postJSON(opts), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_semantic.semantic"></a>[function <span class="apidocSignatureSpan">wechat-api.api_semantic.</span>semantic (uid, opts, callback)](#apidoc.element.wechat-api.api_semantic.semantic)
- description and source-code
```javascript
semantic = function (uid, opts, callback) {
  this.preRequest(this._semantic, arguments);
}
```
- example usage
```shell
...
*   "query":"查一下明天从北京到上海的南航机票",
*   "city":"北京",
*   "category": "flight,hotel"
* }
* '''
* Examples:
* '''
* api.semantic(uid, opts, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```



# <a name="apidoc.module.wechat-api.api_shakearound"></a>[module wechat-api.api_shakearound](#apidoc.module.wechat-api.api_shakearound)

#### <a name="apidoc.element.wechat-api.api_shakearound._addBeaconGroup"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_addBeaconGroup (group, callback)](#apidoc.element.wechat-api.api_shakearound._addBeaconGroup)
- description and source-code
```javascript
_addBeaconGroup = function (group, callback) {
  var url = this.endpoint + '/shakearound/device/group/add?access_token=' + this.token.accessToken;
  this.request(url, postJSON(group), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._addGroupBeacons"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_addGroupBeacons (options, callback)](#apidoc.element.wechat-api.api_shakearound._addGroupBeacons)
- description and source-code
```javascript
_addGroupBeacons = function (options, callback) {
  var url = this.endpoint + '/shakearound/device/group/adddevice?access_token=' + this.token.accessToken;
  this.request(url, postJSON(options), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._addLotteryInfo"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_addLotteryInfo (options, body, callback)](#apidoc.element.wechat-api.api_shakearound._addLotteryInfo)
- description and source-code
```javascript
_addLotteryInfo = function (options, body, callback) {
  var url = this.endpoint + '/shakearound/lottery/addlotteryinfo?&use_template=' + options.use_template + '&logo_url=' + options
.logo_url + '&access_token=' + this.token.accessToken;
  this.request(url, postJSON(body), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._applyBeacons"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_applyBeacons (options, callback)](#apidoc.element.wechat-api.api_shakearound._applyBeacons)
- description and source-code
```javascript
_applyBeacons = function (options, callback) {
  var url = this.endpoint + '/shakearound/device/applyid?access_token=' + this.token.accessToken;
  this.request(url, postJSON(options), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._applyBeaconsStatus"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_applyBeaconsStatus (apply_id, callback)](#apidoc.element.wechat-api.api_shakearound._applyBeaconsStatus)
- description and source-code
```javascript
_applyBeaconsStatus = function (apply_id, callback) {
  var data = {
    apply_id: apply_id
  };
  var url = this.endpoint + '/shakearound/device/applystatus?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._bindBeaconLocation"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_bindBeaconLocation (options, callback)](#apidoc.element.wechat-api.api_shakearound._bindBeaconLocation)
- description and source-code
```javascript
_bindBeaconLocation = function (options, callback) {
  var url = this.endpoint + '/shakearound/device/bindlocation?access_token=' + this.token.accessToken;
  this.request(url, postJSON(options), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._bindBeaconWithPages"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_bindBeaconWithPages (options, callback)](#apidoc.element.wechat-api.api_shakearound._bindBeaconWithPages)
- description and source-code
```javascript
_bindBeaconWithPages = function (options, callback) {
  var url = this.endpoint + '/shakearound/device/bindpage?access_token=' + this.token.accessToken;
  this.request(url, postJSON(options), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._checkShakeAccountStatus"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_checkShakeAccountStatus (callback)](#apidoc.element.wechat-api.api_shakearound._checkShakeAccountStatus)
- description and source-code
```javascript
_checkShakeAccountStatus = function (callback) {
  var url = this.endpoint + '/shakearound/account/auditstatus?access_token=' + this.token.accessToken;
  this.request(url, {dataType: 'json'}, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._createPage"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_createPage (page, callback)](#apidoc.element.wechat-api.api_shakearound._createPage)
- description and source-code
```javascript
_createPage = function (page, callback) {
  var url = this.endpoint + '/shakearound/page/add?access_token=' + this.token.accessToken;
  this.request(url, postJSON(page), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._deleteBeaconGroup"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_deleteBeaconGroup (group_id, callback)](#apidoc.element.wechat-api.api_shakearound._deleteBeaconGroup)
- description and source-code
```javascript
_deleteBeaconGroup = function (group_id, callback) {
  var data = {
    group_id: group_id
  };

  var url = this.endpoint + '/shakearound/device/group/delete?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._deleteGroupBeacons"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_deleteGroupBeacons (options, callback)](#apidoc.element.wechat-api.api_shakearound._deleteGroupBeacons)
- description and source-code
```javascript
_deleteGroupBeacons = function (options, callback) {
  var url = this.endpoint + '/shakearound/device/group/deletedevice?access_token=' + this.token.accessToken;
  this.request(url, postJSON(options), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._deletePage"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_deletePage (page_id, callback)](#apidoc.element.wechat-api.api_shakearound._deletePage)
- description and source-code
```javascript
_deletePage = function (page_id, callback) {
  var data = {page_id: page_id};
  var url = this.endpoint + '/shakearound/page/delete?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._getBeacons"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_getBeacons (options, callback)](#apidoc.element.wechat-api.api_shakearound._getBeacons)
- description and source-code
```javascript
_getBeacons = function (options, callback) {
  var url = this.endpoint + '/shakearound/device/search?access_token=' + this.token.accessToken;
  this.request(url, postJSON(options), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._getDeviceStatistics"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_getDeviceStatistics (options, callback)](#apidoc.element.wechat-api.api_shakearound._getDeviceStatistics)
- description and source-code
```javascript
_getDeviceStatistics = function (options, callback) {
  var url = this.endpoint + '/shakearound/statistics/device?access_token=' + this.token.accessToken;
  this.request(url, postJSON(options), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._getDeviceStatisticsList"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_getDeviceStatisticsList (options, callback)](#apidoc.element.wechat-api.api_shakearound._getDeviceStatisticsList)
- description and source-code
```javascript
_getDeviceStatisticsList = function (options, callback) {
  var url = this.endpoint + '/shakearound/statistics/devicelist?access_token=' + this.token.accessToken;
  this.request(url, postJSON(options), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._getPageStatistics"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_getPageStatistics (options, callback)](#apidoc.element.wechat-api.api_shakearound._getPageStatistics)
- description and source-code
```javascript
_getPageStatistics = function (options, callback) {
  var url = this.endpoint + '/shakearound/statistics/page?access_token=' + this.token.accessToken;
  this.request(url, postJSON(options), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._getPageStatisticsList"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_getPageStatisticsList (options, callback)](#apidoc.element.wechat-api.api_shakearound._getPageStatisticsList)
- description and source-code
```javascript
_getPageStatisticsList = function (options, callback) {
  var url = this.endpoint + '/shakearound/statistics/pagelist?access_token=' + this.token.accessToken;
  this.request(url, postJSON(options), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._getPages"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_getPages (options, callback)](#apidoc.element.wechat-api.api_shakearound._getPages)
- description and source-code
```javascript
_getPages = function (options, callback) {
  var url = this.endpoint + '/shakearound/page/search?access_token=' + this.token.accessToken;
  this.request(url, postJSON(options), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._getShakeInfo"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_getShakeInfo (ticket, callback)](#apidoc.element.wechat-api.api_shakearound._getShakeInfo)
- description and source-code
```javascript
_getShakeInfo = function (ticket, callback) {
  var data = {
    ticket: ticket
  };

  var url = this.endpoint + '/shakearound/user/getshakeinfo?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._listBeaconGroup"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_listBeaconGroup (options, callback)](#apidoc.element.wechat-api.api_shakearound._listBeaconGroup)
- description and source-code
```javascript
_listBeaconGroup = function (options, callback) {
  var url = this.endpoint + '/shakearound/device/group/getlist?access_token=' + this.token.accessToken;
  this.request(url, postJSON(options), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._queryGroupBeacons"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_queryGroupBeacons (options, callback)](#apidoc.element.wechat-api.api_shakearound._queryGroupBeacons)
- description and source-code
```javascript
_queryGroupBeacons = function (options, callback) {
  var url = this.endpoint + '/shakearound/device/group/getdetail?access_token=' + this.token.accessToken;
  this.request(url, postJSON(options), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._registerShakeAccount"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_registerShakeAccount (options, callback)](#apidoc.element.wechat-api.api_shakearound._registerShakeAccount)
- description and source-code
```javascript
_registerShakeAccount = function (options, callback) {
  var url = this.endpoint + '/shakearound/account/register?access_token=' + this.token.accessToken;
  this.request(url, postJSON(options), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._searchBeaconPageRelation"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_searchBeaconPageRelation (options, callback)](#apidoc.element.wechat-api.api_shakearound._searchBeaconPageRelation)
- description and source-code
```javascript
_searchBeaconPageRelation = function (options, callback) {
  var url = this.endpoint + '/shakearound/relation/search?access_token=' + this.token.accessToken;
  this.request(url, postJSON(options), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._setLotterySwitch"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_setLotterySwitch (lotteryId, onoff, callback)](#apidoc.element.wechat-api.api_shakearound._setLotterySwitch)
- description and source-code
```javascript
_setLotterySwitch = function (lotteryId, onoff, callback) {
  var url = this.endpoint + '/shakearound/lottery/setlotteryswitch?lottery_id=' + lotteryId + '&onoff=' + onoff + '&access_token
=' + this.token.accessToken;
  this.request(url, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._setPrizeBucket"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_setPrizeBucket (options, callback)](#apidoc.element.wechat-api.api_shakearound._setPrizeBucket)
- description and source-code
```javascript
_setPrizeBucket = function (options, callback) {
  var url = this.endpoint + '/shakearound/lottery/setprizebucket?access_token=' + this.token.accessToken;
  this.request(url, postJSON(options), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._updateBeacon"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_updateBeacon (options, callback)](#apidoc.element.wechat-api.api_shakearound._updateBeacon)
- description and source-code
```javascript
_updateBeacon = function (options, callback) {
  var url = this.endpoint + '/shakearound/device/update?access_token=' + this.token.accessToken;
  this.request(url, postJSON(options), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._updateBeaconGroup"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_updateBeaconGroup (group, callback)](#apidoc.element.wechat-api.api_shakearound._updateBeaconGroup)
- description and source-code
```javascript
_updateBeaconGroup = function (group, callback) {
  var url = this.endpoint + '/shakearound/device/group/update?access_token=' + this.token.accessToken;
  this.request(url, postJSON(group), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._updatePage"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_updatePage (page, callback)](#apidoc.element.wechat-api.api_shakearound._updatePage)
- description and source-code
```javascript
_updatePage = function (page, callback) {
  var url = this.endpoint + '/shakearound/page/update?access_token=' + this.token.accessToken;
  this.request(url, postJSON(page), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound._uploadPageIcon"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>_uploadPageIcon (filepath, callback)](#apidoc.element.wechat-api.api_shakearound._uploadPageIcon)
- description and source-code
```javascript
_uploadPageIcon = function (filepath, callback) {
  var that = this;
  fs.stat(filepath, function (err, stat) {
    if (err) {
      return callback(err);
    }
    var form = formstream();
    form.file('media', filepath, path.basename(filepath), stat.size);
    var url = this.endpoint + '/shakearound/material/add?access_token=' + that.token.accessToken;
    var opts = {
      dataType: 'json',
      type: 'POST',
      timeout: 60000, // 60秒超时
      headers: form.headers(),
      stream: form
    };
    that.request(url, opts, callback);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound.addBeaconGroup"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>addBeaconGroup ()](#apidoc.element.wechat-api.api_shakearound.addBeaconGroup)
- description and source-code
```javascript
addBeaconGroup = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
* 新建设备分组，每个帐号下最多只有100个分组。
* group:
* {
*   group_name: 'test'
* }
* Examples:
* '''
* api.addBeaconGroup(group, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.addGroupBeacons"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>addGroupBeacons ()](#apidoc.element.wechat-api.api_shakearound.addGroupBeacons)
- description and source-code
```javascript
addGroupBeacons = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
*      "minor": 1223
*    }
*  ]
* }
* '''
* Examples:
* '''
* api.addGroupBeacons(options, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.addLotteryInfo"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>addLotteryInfo ()](#apidoc.element.wechat-api.api_shakearound.addLotteryInfo)
- description and source-code
```javascript
addLotteryInfo = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
*   "total": 10,
*   "jump_url": "https://lodejs.org",
*   "key": "u5pPq38tQP97yGn8iZxbBsfWvbn37poP"
* }
* '''
* Examples:
* '''
* api.addLotteryInfo(options, body, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.applyBeacons"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>applyBeacons ()](#apidoc.element.wechat-api.api_shakearound.applyBeacons)
- description and source-code
```javascript
applyBeacons = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
*   "comment":"测试专用",
*   "poi_id":1234
* }
* '''
*
* Examples:
* '''
* api.applyBeacons(options, callback);
* '''
*
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.applyBeaconsStatus"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>applyBeaconsStatus ()](#apidoc.element.wechat-api.api_shakearound.applyBeaconsStatus)
- description and source-code
```javascript
applyBeaconsStatus = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
* {
*   "apply_id": 12345
* }
* '''
*
* Examples:
* '''
* api.applyBeaconsStatus(apply_id, callback);
* '''
*
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.bindBeaconLocation"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>bindBeaconLocation ()](#apidoc.element.wechat-api.api_shakearound.bindBeaconLocation)
- description and source-code
```javascript
bindBeaconLocation = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
*     "minor": 1223
*   },
*   "poi_id": 1231
* }
* '''
* Examples:
* '''
* api.bindBeaconLocation(options, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.bindBeaconWithPages"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>bindBeaconWithPages ()](#apidoc.element.wechat-api.api_shakearound.bindBeaconWithPages)
- description and source-code
```javascript
bindBeaconWithPages = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
*    "minor":1223
*  },
*  "page_ids":[12345, 23456, 334567]
* }
* '''
* Examples:
* '''
* api.bindBeaconWithPages(options, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.checkShakeAccountStatus"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>checkShakeAccountStatus ()](#apidoc.element.wechat-api.api_shakearound.checkShakeAccountStatus)
- description and source-code
```javascript
checkShakeAccountStatus = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
/**
* 查询审核状态
* 接口说明：
* 查询已经提交的开通摇一摇周边功能申请的审核状态。在申请提交后，工作人员会在三个工作日内完成审核。
* 详情请参见：http://mp.weixin.qq.com/wiki/13/025f1d471dc999928340161c631c6635.html
* Examples:
* '''
* api.checkShakeAccountStatus(callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.createPage"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>createPage ()](#apidoc.element.wechat-api.api_shakearound.createPage)
- description and source-code
```javascript
createPage = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
*   "comment":"数据示例",
*   "icon_url":"http://shp.qpic.cn/wx_shake_bus/0/14288351768a23d76e7636b56440172120529e8252/120"
*   //调用uploadPageIcon函数获取到该URL
* }
* '''
* Examples:
* '''
* api.createPage(page, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.deleteBeaconGroup"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>deleteBeaconGroup ()](#apidoc.element.wechat-api.api_shakearound.deleteBeaconGroup)
- description and source-code
```javascript
deleteBeaconGroup = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
* 删除设备分组，若分组中还存在设备，则不能删除成功。需把设备移除以后，才能删除。
* group:
* {
*   group_id: 123
* }
* Examples:
* '''
* api.deleteBeaconGroup(group_id, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.deleteGroupBeacons"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>deleteGroupBeacons ()](#apidoc.element.wechat-api.api_shakearound.deleteGroupBeacons)
- description and source-code
```javascript
deleteGroupBeacons = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
*      "minor": 1223
*    }
*  ]
* }
* '''
* Examples:
* '''
* api.deleteGroupBeacons(options, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.deletePage"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>deletePage ()](#apidoc.element.wechat-api.api_shakearound.deletePage)
- description and source-code
```javascript
deletePage = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
* '''
* {
*   "page_id": 34567
* }
* '''
* Examples:
* '''
* api.deletePage(page_id, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.getBeacons"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>getBeacons ()](#apidoc.element.wechat-api.api_shakearound.getBeacons)
- description and source-code
```javascript
getBeacons = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
*   "apply_id": 1231,
*   "begin": 0,
*   "count": 3
* }
* '''
* Examples:
* '''
* api.getBeacons(options, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.getDeviceStatistics"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>getDeviceStatistics ()](#apidoc.element.wechat-api.api_shakearound.getDeviceStatistics)
- description and source-code
```javascript
getDeviceStatistics = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
*   },
*   "begin_date": 12313123311,
*   "end_date": 123123131231
* }
* '''
* Examples:
* '''
* api.getDeviceStatistics(options, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.getDeviceStatisticsList"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>getDeviceStatisticsList ()](#apidoc.element.wechat-api.api_shakearound.getDeviceStatisticsList)
- description and source-code
```javascript
getDeviceStatisticsList = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
* {
*   date: 1438704000,
*   page_index: 1
* }
* '''
* Examples:
* '''
* api.getDeviceStatisticsList(options, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.getPageStatistics"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>getPageStatistics ()](#apidoc.element.wechat-api.api_shakearound.getPageStatistics)
- description and source-code
```javascript
getPageStatistics = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
*   "page_id": 12345,
*   "begin_date": 12313123311,
*   "end_date": 123123131231
* }
* '''
* Examples:
* '''
* api.getPageStatistics(options, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.getPageStatisticsList"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>getPageStatisticsList ()](#apidoc.element.wechat-api.api_shakearound.getPageStatisticsList)
- description and source-code
```javascript
getPageStatisticsList = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
* {
*   date: 1425139200,
*   page_index: 1
* }
* '''
* Examples:
* '''
* api.getPageStatisticsList(options, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.getPages"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>getPages ()](#apidoc.element.wechat-api.api_shakearound.getPages)
- description and source-code
```javascript
getPages = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shakearound.getShakeInfo"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>getShakeInfo ()](#apidoc.element.wechat-api.api_shakearound.getShakeInfo)
- description and source-code
```javascript
getShakeInfo = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
* '''
* {
*   "ticket":”6ab3d8465166598a5f4e8c1b44f44645”
* }
* '''
* Examples:
* '''
* api.getShakeInfo(ticket, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.getShakehbConfig"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>getShakehbConfig (openid, lotteryId, key)](#apidoc.element.wechat-api.api_shakearound.getShakehbConfig)
- description and source-code
```javascript
getShakehbConfig = function (openid, lotteryId, key) {
  var params = {
    openid: openid,
    lottery_id: lotteryId,
    noncestr: Math.random().toString(36).substr(2, 15)
  };

  var query = Object.keys(params).sort().map(function(key) {
    return key + '=' + params[key];
  }).join('&');

  query += '&key=' + key;
  params.sign = crypto.createHash('md5').update(query).digest('hex').toUpperCase();

  return params;
}
```
- example usage
```shell
...
/**
* 获取红包JSAPI参数
* 接口说明:
* 用于在第三方页面中，通过调用JSAPI来触发用户抽红包的操作。
* 详情请参见：http://mp.weixin.qq.com/wiki/12/9738788d171724b080b52f6e41490cb4.html
* Examples:
* '''
* api.getShakehbConfig(openid, lotteryId, key);
* '''
* Return:
* '''
* {
*   "openid": "o-hVKuNknQQBZFDlbE8eibQzIX3o",
*   "lottery_id": "5794560"
*   "noncestr": "5K8264ILTKCH16CQ2502SI8ZNMTM67VS"
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.listBeaconGroup"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>listBeaconGroup ()](#apidoc.element.wechat-api.api_shakearound.listBeaconGroup)
- description and source-code
```javascript
listBeaconGroup = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
* options:
* {
*   begin: 0,
*   count: 10
* }
* Examples:
* '''
* api.listBeaconGroup(options, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.queryGroupBeacons"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>queryGroupBeacons ()](#apidoc.element.wechat-api.api_shakearound.queryGroupBeacons)
- description and source-code
```javascript
queryGroupBeacons = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
* {
 *  group_id: 123,
*   begin: 0,
*   count: 10
* }
* Examples:
* '''
* api.queryGroupBeacons(options, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.registerShakeAccount"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>registerShakeAccount ()](#apidoc.element.wechat-api.api_shakearound.registerShakeAccount)
- description and source-code
```javascript
registerShakeAccount = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
*  ],
*  "apply_reason": "test"
* }
* '''
*
* Examples:
* '''
* api.registerShakeAccount(options, callback);
* '''
*
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.searchBeaconPageRelation"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>searchBeaconPageRelation ()](#apidoc.element.wechat-api.api_shakearound.searchBeaconPageRelation)
- description and source-code
```javascript
searchBeaconPageRelation = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
*  "type": 2,
*  "page_id": 11101,
*  "begin": 0,
*  "count": 3
* }
* Examples:
* '''
* api.searchBeaconPageRelation(options, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.setLotterySwitch"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>setLotterySwitch ()](#apidoc.element.wechat-api.api_shakearound.setLotterySwitch)
- description and source-code
```javascript
setLotterySwitch = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
/**
* 设置红包活动抽奖开关
* 接口说明:
* 开发者实时控制红包活动抽奖的开启和关闭。
* 详情请参见：http://mp.weixin.qq.com/wiki/12/9738788d171724b080b52f6e41490cb4.html
* Examples:
* '''
* api.setLotterySwitch(lotteryId, onoff, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.setPrizeBucket"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>setPrizeBucket ()](#apidoc.element.wechat-api.api_shakearound.setPrizeBucket)
- description and source-code
```javascript
setPrizeBucket = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
*   "prize_info_list": [{
*     "ticket": "v1|ZiPs2l0hpMBp3uwGI1rwp45vOdz/V/zQ/00jP9MeWT+e47/q1FJjwCIP34frSjzOxAEzJ7k2CtAg1pmcShvkChBWqbThxPm6MBuzceoHtj79iHuHaEn0WAO
+j4sXnXnbGswFOlDYWg1ngvrRYnCY3g==",
*   }]
* }
* '''
* Examples:
* '''
* api.setPrizeBucket(options, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.updateBeacon"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>updateBeacon ()](#apidoc.element.wechat-api.api_shakearound.updateBeacon)
- description and source-code
```javascript
updateBeacon = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
*    "minor": 1223
*  },
*  "comment": "test"
* }
* '''
* Examples:
* '''
* api.updateBeacon(options, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.updateBeaconGroup"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>updateBeaconGroup ()](#apidoc.element.wechat-api.api_shakearound.updateBeaconGroup)
- description and source-code
```javascript
updateBeaconGroup = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
* group:
* {
*   group_id: 123,
*   group_name: 'test update'
* }
* Examples:
* '''
* api.updateBeaconGroup(group, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.updatePage"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>updatePage ()](#apidoc.element.wechat-api.api_shakearound.updatePage)
- description and source-code
```javascript
updatePage = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
*   "comment":"数据示例",
*   "icon_url":"http://shp.qpic.cn/wx_shake_bus/0/14288351768a23d76e7636b56440172120529e8252/120"
*   //调用uploadPageIcon函数获取到该URL
* }
* '''
* Examples:
* '''
* api.updatePage(page, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shakearound.uploadPageIcon"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shakearound.</span>uploadPageIcon ()](#apidoc.element.wechat-api.api_shakearound.uploadPageIcon)
- description and source-code
```javascript
uploadPageIcon = function () {
  this.preRequest(this['_' + name], arguments);
}
```
- example usage
```shell
...
* 上传图片素材
* 接口说明：
* 上传在摇一摇页面展示的图片素材，素材保存在微信侧服务器上。
* 格式限定为：jpg,jpeg,png,gif，图片大小建议120px*120 px，限制不超过200 px *200 px，图片需为正方形。
* 详情请参见：http://mp.weixin.qq.com/wiki/5/e997428269ff189d8f9a4b9e177be2d9.html
* Examples:
* '''
* api.uploadPageIcon('filepath', callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```



# <a name="apidoc.module.wechat-api.api_shop_common"></a>[module wechat-api.api_shop_common](#apidoc.module.wechat-api.api_shop_common)

#### <a name="apidoc.element.wechat-api.api_shop_common._uploadPicture"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_common.</span>_uploadPicture (filepath, callback)](#apidoc.element.wechat-api.api_shop_common._uploadPicture)
- description and source-code
```javascript
_uploadPicture = function (filepath, callback) {
  var basename = path.basename(filepath);
  var url = this.endpoint + '/merchant/common/upload_img?access_token=' +
    this.token.accessToken + '&filename=' + basename;
  var reader = fs.createReadStream(filepath);
  var opts = {
    dataType: 'json',
    type: 'POST',
    stream: reader
  };
  this.request(url, opts, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_common.uploadPicture"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_common.</span>uploadPicture (filepath, callback)](#apidoc.element.wechat-api.api_shop_common.uploadPicture)
- description and source-code
```javascript
uploadPicture = function (filepath, callback) {
  this.preRequest(this._uploadPicture, arguments);
}
```
- example usage
```shell
...
var wrapper = util.wrapper;

/**
* 上传图片
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.uploadPicture('/path/to/your/img.jpg', callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```



# <a name="apidoc.module.wechat-api.api_shop_express"></a>[module wechat-api.api_shop_express](#apidoc.module.wechat-api.api_shop_express)

#### <a name="apidoc.element.wechat-api.api_shop_express._addExpressTemplate"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_express.</span>_addExpressTemplate (express, callback)](#apidoc.element.wechat-api.api_shop_express._addExpressTemplate)
- description and source-code
```javascript
_addExpressTemplate = function (express, callback) {
  var url = this.endpoint + '/merchant/express/add?access_token=' + this.token.accessToken;
  this.request(url, postJSON(express), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_express._deleteExpressTemplate"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_express.</span>_deleteExpressTemplate (templateId, callback)](#apidoc.element.wechat-api.api_shop_express._deleteExpressTemplate)
- description and source-code
```javascript
_deleteExpressTemplate = function (templateId, callback) {
  var data = {
    template_id: templateId
  };
  var url = this.endpoint + '/merchant/express/del?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_express._getAllExpressTemplates"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_express.</span>_getAllExpressTemplates (callback)](#apidoc.element.wechat-api.api_shop_express._getAllExpressTemplates)
- description and source-code
```javascript
_getAllExpressTemplates = function (callback) {
  var url = this.endpoint + '/merchant/express/getall?access_token=' + this.token.accessToken;
  this.request(url, {dataType: 'json'}, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_express._getExpressTemplateById"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_express.</span>_getExpressTemplateById (templateId, callback)](#apidoc.element.wechat-api.api_shop_express._getExpressTemplateById)
- description and source-code
```javascript
_getExpressTemplateById = function (templateId, callback) {
  var data = {
    template_id: templateId
  };
  var url = this.endpoint + '/merchant/express/getbyid?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_express._updateExpressTemplate"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_express.</span>_updateExpressTemplate (template, callback)](#apidoc.element.wechat-api.api_shop_express._updateExpressTemplate)
- description and source-code
```javascript
_updateExpressTemplate = function (template, callback) {
  var url = this.endpoint + '/merchant/express/del?access_token=' + this.token.accessToken;
  this.request(url, postJSON(template), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_express.addExpressTemplate"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_express.</span>addExpressTemplate (express, callback)](#apidoc.element.wechat-api.api_shop_express.addExpressTemplate)
- description and source-code
```javascript
addExpressTemplate = function (express, callback) {
  this.preRequest(this._addExpressTemplate, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_express.deleteExpressTemplate"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_express.</span>deleteExpressTemplate (templateId, callback)](#apidoc.element.wechat-api.api_shop_express.deleteExpressTemplate)
- description and source-code
```javascript
deleteExpressTemplate = function (templateId, callback) {
  this.preRequest(this._deleteExpressTemplate, arguments);
}
```
- example usage
```shell
...
};

/**
* 修改邮费模板
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.deleteExpressTemplate(templateId, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shop_express.getAllExpressTemplates"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_express.</span>getAllExpressTemplates (callback)](#apidoc.element.wechat-api.api_shop_express.getAllExpressTemplates)
- description and source-code
```javascript
getAllExpressTemplates = function (callback) {
  this.preRequest(this._getAllExpressTemplates, arguments);
}
```
- example usage
```shell
...
};

/**
* 获取所有邮费模板的未封装版本
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.getAllExpressTemplates(callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shop_express.getExpressTemplateById"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_express.</span>getExpressTemplateById (templateId, callback)](#apidoc.element.wechat-api.api_shop_express.getExpressTemplateById)
- description and source-code
```javascript
getExpressTemplateById = function (templateId, callback) {
  this.preRequest(this._getExpressTemplateById, arguments);
}
```
- example usage
```shell
...
};

/**
* 获取指定ID的邮费模板
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.getExpressTemplateById(templateId, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shop_express.updateExpressTemplate"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_express.</span>updateExpressTemplate (template, callback)](#apidoc.element.wechat-api.api_shop_express.updateExpressTemplate)
- description and source-code
```javascript
updateExpressTemplate = function (template, callback) {
  this.preRequest(this._updateExpressTemplate, arguments);
}
```
- example usage
```shell
...
};

/**
* 修改邮费模板
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.updateExpressTemplate(template, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Express:
...
```



# <a name="apidoc.module.wechat-api.api_shop_goods"></a>[module wechat-api.api_shop_goods](#apidoc.module.wechat-api.api_shop_goods)

#### <a name="apidoc.element.wechat-api.api_shop_goods._createGoods"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>_createGoods (goods, callback)](#apidoc.element.wechat-api.api_shop_goods._createGoods)
- description and source-code
```javascript
_createGoods = function (goods, callback) {
  var url = this.endpoint + '/merchant/create?access_token=' + this.token.accessToken;
  this.request(url, postJSON(goods), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_goods._deleteGoods"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>_deleteGoods (productId, callback)](#apidoc.element.wechat-api.api_shop_goods._deleteGoods)
- description and source-code
```javascript
_deleteGoods = function (productId, callback) {
  var data = {
    'product_id': productId
  };
  var url = this.endpoint + '/merchant/del?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_goods._getGoods"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>_getGoods (productId, callback)](#apidoc.element.wechat-api.api_shop_goods._getGoods)
- description and source-code
```javascript
_getGoods = function (productId, callback) {
  var url = this.endpoint + '/merchant/get?product_id=' + productId + '&access_token=' + this.token.accessToken;
  this.request(url, {dataType: 'json'}, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_goods._getGoodsByStatus"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>_getGoodsByStatus (status, callback)](#apidoc.element.wechat-api.api_shop_goods._getGoodsByStatus)
- description and source-code
```javascript
_getGoodsByStatus = function (status, callback) {
  var data = {status: status};
  var url = this.endpoint + '/merchant/getbystatus?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_goods._getProperties"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>_getProperties (catId, callback)](#apidoc.element.wechat-api.api_shop_goods._getProperties)
- description and source-code
```javascript
_getProperties = function (catId, callback) {
  var data = {
    cate_id: catId
  };
  var url = this.endpoint + '/merchant/category/getproperty?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_goods._getSKUs"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>_getSKUs (catId, callback)](#apidoc.element.wechat-api.api_shop_goods._getSKUs)
- description and source-code
```javascript
_getSKUs = function (catId, callback) {
  var data = {
    cate_id: catId
  };
  var url = this.endpoint + '/merchant/category/getsku?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_goods._getSubCats"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>_getSubCats (catId, callback)](#apidoc.element.wechat-api.api_shop_goods._getSubCats)
- description and source-code
```javascript
_getSubCats = function (catId, callback) {
  var data = {
    cate_id: catId
  };
  var url = this.endpoint + '/merchant/category/getsub?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_goods._updateGoods"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>_updateGoods (goods, callback)](#apidoc.element.wechat-api.api_shop_goods._updateGoods)
- description and source-code
```javascript
_updateGoods = function (goods, callback) {
  var url = this.endpoint + '/merchant/update?access_token=' + this.token.accessToken;
  this.request(url, postJSON(goods), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_goods._updateGoodsStatus"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>_updateGoodsStatus (productId, status, callback)](#apidoc.element.wechat-api.api_shop_goods._updateGoodsStatus)
- description and source-code
```javascript
_updateGoodsStatus = function (productId, status, callback) {
  var data = {
    product_id: productId,
    status: status
  };
  var url = this.endpoint + '/merchant/modproductstatus?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_goods.createGoods"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>createGoods (goods, callback)](#apidoc.element.wechat-api.api_shop_goods.createGoods)
- description and source-code
```javascript
createGoods = function (goods, callback) {
  this.preRequest(this._createGoods, arguments);
}
```
- example usage
```shell
...
var postJSON = util.postJSON;

/**
* 增加商品
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.createGoods(goods, callback);
* '''
* Goods:
* '''
* {
*  "product_base":{
*    "category_id":[
*      "537074298"
...
```

#### <a name="apidoc.element.wechat-api.api_shop_goods.deleteGoods"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>deleteGoods (productId, callback)](#apidoc.element.wechat-api.api_shop_goods.deleteGoods)
- description and source-code
```javascript
deleteGoods = function (productId, callback) {
  this.preRequest(this._deleteGoods, arguments);
}
```
- example usage
```shell
...
};

/**
* 删除商品
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.deleteGoods(productId, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shop_goods.getGoods"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>getGoods (productId, callback)](#apidoc.element.wechat-api.api_shop_goods.getGoods)
- description and source-code
```javascript
getGoods = function (productId, callback) {
  this.preRequest(this._getGoods, arguments);
}
```
- example usage
```shell
...
};

/**
* 查询商品
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.getGoods(productId, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shop_goods.getGoodsByStatus"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>getGoodsByStatus (status, callback)](#apidoc.element.wechat-api.api_shop_goods.getGoodsByStatus)
- description and source-code
```javascript
getGoodsByStatus = function (status, callback) {
  this.preRequest(this._getGoodsByStatus, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_goods.getProperties"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>getProperties (catId, callback)](#apidoc.element.wechat-api.api_shop_goods.getProperties)
- description and source-code
```javascript
getProperties = function (catId, callback) {
  this.preRequest(this._getProperties, arguments);
}
```
- example usage
```shell
...
};

/**
* 获取指定分类的所有属性
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.getProperties(catId, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shop_goods.getSKUs"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>getSKUs (catId, callback)](#apidoc.element.wechat-api.api_shop_goods.getSKUs)
- description and source-code
```javascript
getSKUs = function (catId, callback) {
  this.preRequest(this._getSKUs, arguments);
}
```
- example usage
```shell
...
};

/**
* 获取指定子分类的所有SKU
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.getSKUs(catId, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shop_goods.getSubCats"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>getSubCats (catId, callback)](#apidoc.element.wechat-api.api_shop_goods.getSubCats)
- description and source-code
```javascript
getSubCats = function (catId, callback) {
  this.preRequest(this._getSubCats, arguments);
}
```
- example usage
```shell
...
};

/**
* 获取指定分类的所有子分类
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.getSubCats(catId, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shop_goods.updateGoods"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>updateGoods (goods, callback)](#apidoc.element.wechat-api.api_shop_goods.updateGoods)
- description and source-code
```javascript
updateGoods = function (goods, callback) {
  this.preRequest(this._updateGoods, arguments);
}
```
- example usage
```shell
...
};

/**
* 修改商品
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.updateGoods(goods, callback);
* '''
* Goods:
* '''
* {
*  "product_id":"pDF3iY6Kr_BV_CXaiYysoGqJhppQ",
*  "product_base":{
*    "category_id":[
...
```

#### <a name="apidoc.element.wechat-api.api_shop_goods.updateGoodsStatus"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_goods.</span>updateGoodsStatus (productId, status, callback)](#apidoc.element.wechat-api.api_shop_goods.updateGoodsStatus)
- description and source-code
```javascript
updateGoodsStatus = function (productId, status, callback) {
  this.preRequest(this._updateGoodsStatus, arguments);
}
```
- example usage
```shell
...
};

/**
* 商品上下架
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.updateGoodsStatus(productId, status, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```



# <a name="apidoc.module.wechat-api.api_shop_group"></a>[module wechat-api.api_shop_group](#apidoc.module.wechat-api.api_shop_group)

#### <a name="apidoc.element.wechat-api.api_shop_group._createGoodsGroup"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_group.</span>_createGoodsGroup (groupName, productList, callback)](#apidoc.element.wechat-api.api_shop_group._createGoodsGroup)
- description and source-code
```javascript
_createGoodsGroup = function (groupName, productList, callback) {
  var data = {
    'group_detail': {
      'group_name': groupName,
      'product_list': productList && productList.length ? productList: []
    }
  };
  var url = this.endpoint + '/merchant/group/add?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_group._deleteGoodsGroup"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_group.</span>_deleteGoodsGroup (groupId, callback)](#apidoc.element.wechat-api.api_shop_group._deleteGoodsGroup)
- description and source-code
```javascript
_deleteGoodsGroup = function (groupId, callback) {
  var data = {
    'group_id': groupId
  };
  var url = this.endpoint + '/merchant/group/del?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_group._getAllGroups"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_group.</span>_getAllGroups (callback)](#apidoc.element.wechat-api.api_shop_group._getAllGroups)
- description and source-code
```javascript
_getAllGroups = function (callback) {
  var url = this.endpoint + '/merchant/group/getall?access_token=' + this.token.accessToken;
  this.request(url, {dataType: 'json'}, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_group._getGroupById"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_group.</span>_getGroupById (groupId, callback)](#apidoc.element.wechat-api.api_shop_group._getGroupById)
- description and source-code
```javascript
_getGroupById = function (groupId, callback) {
  var data = {
    'group_id': groupId
  };
  var url = this.endpoint + '/merchant/group/getbyid?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_group._updateGoodsForGroup"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_group.</span>_updateGoodsForGroup (groupId, addProductList, delProductList, callback)](#apidoc.element.wechat-api.api_shop_group._updateGoodsForGroup)
- description and source-code
```javascript
_updateGoodsForGroup = function (groupId, addProductList, delProductList, callback) {
  var data = {
    'group_id': groupId,
    'product': []
  };

  if (addProductList && addProductList.length) {
    addProductList.forEach(function (val) {
      data.product.push({
        'product_id': val,
        'mod_action': 1
      });
    });
  }

  if (delProductList && delProductList.length) {
    delProductList.forEach(function (val) {
      data.product.push({
        'product_id': val,
        'mod_action': 0
      });
    });
  }

  var url = this.endpoint + '/merchant/group/productmod?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_group._updateGoodsGroup"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_group.</span>_updateGoodsGroup (groupId, groupName, callback)](#apidoc.element.wechat-api.api_shop_group._updateGoodsGroup)
- description and source-code
```javascript
_updateGoodsGroup = function (groupId, groupName, callback) {
  var data = {
    'group_id': groupId,
    'group_name': groupName
  };
  var url = this.endpoint + '/merchant/group/propertymod?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_group.createGoodsGroup"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_group.</span>createGoodsGroup (groupName, productList, callback)](#apidoc.element.wechat-api.api_shop_group.createGoodsGroup)
- description and source-code
```javascript
createGoodsGroup = function (groupName, productList, callback) {
  this.preRequest(this._createGoodsGroup, arguments);
}
```
- example usage
```shell
...
var postJSON = util.postJSON;

/**
* 创建商品分组
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.createGoodsGroup(groupName, productList, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shop_group.deleteGoodsGroup"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_group.</span>deleteGoodsGroup (groupId, callback)](#apidoc.element.wechat-api.api_shop_group.deleteGoodsGroup)
- description and source-code
```javascript
deleteGoodsGroup = function (groupId, callback) {
  this.preRequest(this._deleteGoodsGroup, arguments);
}
```
- example usage
```shell
...
};

/**
* 删除商品分组
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.deleteGoodsGroup(groupId, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shop_group.getAllGroups"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_group.</span>getAllGroups (callback)](#apidoc.element.wechat-api.api_shop_group.getAllGroups)
- description and source-code
```javascript
getAllGroups = function (callback) {
  this.preRequest(this._getAllGroups, arguments);
}
```
- example usage
```shell
...
};

/**
* 获取所有商品分组
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.getAllGroups(callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shop_group.getGroupById"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_group.</span>getGroupById (groupId, callback)](#apidoc.element.wechat-api.api_shop_group.getGroupById)
- description and source-code
```javascript
getGroupById = function (groupId, callback) {
  this.preRequest(this._getGroupById, arguments);
}
```
- example usage
```shell
...
};

/**
* 根据ID获取商品分组
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.getGroupById(groupId, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shop_group.updateGoodsForGroup"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_group.</span>updateGoodsForGroup (groupId, addProductList, delProductList, callback)](#apidoc.element.wechat-api.api_shop_group.updateGoodsForGroup)
- description and source-code
```javascript
updateGoodsForGroup = function (groupId, addProductList, delProductList, callback) {
  this.preRequest(this._updateGoodsForGroup, arguments);
}
```
- example usage
```shell
...
};

/**
* 修改商品分组内的商品
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.updateGoodsForGroup(groupId, addProductList, delProductList, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shop_group.updateGoodsGroup"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_group.</span>updateGoodsGroup (groupId, groupName, callback)](#apidoc.element.wechat-api.api_shop_group.updateGoodsGroup)
- description and source-code
```javascript
updateGoodsGroup = function (groupId, groupName, callback) {
  this.preRequest(this._updateGoodsGroup, arguments);
}
```
- example usage
```shell
...
};

/**
* 修改商品分组属性
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.updateGoodsGroup(groupId, groupName, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```



# <a name="apidoc.module.wechat-api.api_shop_order"></a>[module wechat-api.api_shop_order](#apidoc.module.wechat-api.api_shop_order)

#### <a name="apidoc.element.wechat-api.api_shop_order._closeOrder"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_order.</span>_closeOrder (orderId, callback)](#apidoc.element.wechat-api.api_shop_order._closeOrder)
- description and source-code
```javascript
_closeOrder = function (orderId, callback) {
  var data = {
    'order_id': orderId
  };
  var url = this.endpoint + '/merchant/order/close?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_order._getOrderById"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_order.</span>_getOrderById (orderId, callback)](#apidoc.element.wechat-api.api_shop_order._getOrderById)
- description and source-code
```javascript
_getOrderById = function (orderId, callback) {
  var data = {
    'order_id': orderId
  };
  var url = this.endpoint + '/merchant/order/getbyid?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_order._getOrdersByStatus"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_order.</span>_getOrdersByStatus (status, beginTime, endTime, callback)](#apidoc.element.wechat-api.api_shop_order._getOrdersByStatus)
- description and source-code
```javascript
_getOrdersByStatus = function (status, beginTime, endTime, callback) {
  var data = {};
  if (arguments.length === 1 && typeof status === 'function') {
    // (callback);
    callback = status;
  } else if (arguments.length === 2 && typeof beginTime === 'function') {
    callback = beginTime;
    if (typeof status === 'number') {
      // (status, callback)
      data.status = status;
    } else if (status instanceof Date) {
      data.begintime = Math.round(status.getTime() / 1000);
      data.endtime = Math.round(new Date().getTime() / 1000);
    } else {
      throw new Error('first parameter must be Number or Date');
    }
  } else if (arguments.length === 3 && typeof endTime === 'function') {
    callback = endTime;
    if (typeof status === 'number' && beginTime instanceof Date) {
      data.status = status;
      data.begintime = Math.round(beginTime.getTime() / 1000);
      data.endtime = Math.round(new Date().getTime() / 1000);
    } else {
      throw new Error('first parameter must be Number and second parameter must be Date');
    }
  } else if (arguments.length === 4) {
    data.status = status;
    data.begintime = Math.round(beginTime.getTime() / 1000);
    data.endtime = Math.round(endTime.getTime() / 1000);
  }
  var url = this.endpoint + '/merchant/order/getbyfilter?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_order._setExpressForOrder"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_order.</span>_setExpressForOrder (orderId, deliveryCompany, deliveryTrackNo, callback)](#apidoc.element.wechat-api.api_shop_order._setExpressForOrder)
- description and source-code
```javascript
_setExpressForOrder = function (orderId, deliveryCompany, deliveryTrackNo, callback) {
  var data = {
    'order_id': orderId,
    'delivery_company': deliveryCompany,
    'delivery_track_no': deliveryTrackNo
  };
  var url = this.endpoint + '/merchant/order/setdelivery?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_order.closeOrder"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_order.</span>closeOrder (orderId, callback)](#apidoc.element.wechat-api.api_shop_order.closeOrder)
- description and source-code
```javascript
closeOrder = function (orderId, callback) {
  this.preRequest(this._closeOrder, arguments);
}
```
- example usage
```shell
...
};

/**
* 关闭订单
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.closeOrder(orderId, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shop_order.getOrderById"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_order.</span>getOrderById (orderId, callback)](#apidoc.element.wechat-api.api_shop_order.getOrderById)
- description and source-code
```javascript
getOrderById = function (orderId, callback) {
  this.preRequest(this._getOrderById, arguments);
}
```
- example usage
```shell
...
var postJSON = util.postJSON;

/**
* 根据订单Id获取订单详情
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.getOrderById(orderId, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shop_order.getOrdersByStatus"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_order.</span>getOrdersByStatus ()](#apidoc.element.wechat-api.api_shop_order.getOrdersByStatus)
- description and source-code
```javascript
getOrdersByStatus = function () {
  this.preRequest(this._getOrdersByStatus, arguments);
}
```
- example usage
```shell
...
};

/**
* 根据订单状态/创建时间获取订单详情
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.getOrdersByStatus([status,] [beginTime,] [endTime,] callback);
* '''
* Usage:
* 当只传入callback参数时，查询所有状态，所有时间的订单
* 当传入两个参数，第一个参数为Number类型，第二个参数为callback时，查询指定状态，所有时间的订单
* 当传入两个参数，第一个参数为Date类型，第二个参数为callback时，查询所有状态，指定订单创建起始时间的订单(待测试)
* 当传入三个参数，第一参数为订单状态码，第二参数为订单创建起始时间，第三参数为callback
* 当传入四个参数，第一参数为订单状态码，第二参数为订单创建起始时间，第三参数为订单创建终止时间，第四参数为callback
...
```

#### <a name="apidoc.element.wechat-api.api_shop_order.setExpressForOrder"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_order.</span>setExpressForOrder (orderId, deliveryCompany, deliveryTrackNo, callback)](#apidoc.element.wechat-api.api_shop_order.setExpressForOrder)
- description and source-code
```javascript
setExpressForOrder = function (orderId, deliveryCompany, deliveryTrackNo, callback) {
  this.preRequest(this._setExpressForOrder, arguments);
}
```
- example usage
```shell
...
};

/**
* 设置订单发货信息
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.setExpressForOrder(orderId, deliveryCompany, deliveryTrackNo, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```



# <a name="apidoc.module.wechat-api.api_shop_shelf"></a>[module wechat-api.api_shop_shelf](#apidoc.module.wechat-api.api_shop_shelf)

#### <a name="apidoc.element.wechat-api.api_shop_shelf._createShelf"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_shelf.</span>_createShelf (shelf, callback)](#apidoc.element.wechat-api.api_shop_shelf._createShelf)
- description and source-code
```javascript
_createShelf = function (shelf, callback) {
  var url = this.endpoint + '/merchant/shelf/add?access_token=' + this.token.accessToken;
  this.request(url, postJSON(shelf), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_shelf._deleteShelf"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_shelf.</span>_deleteShelf (shelfId, callback)](#apidoc.element.wechat-api.api_shop_shelf._deleteShelf)
- description and source-code
```javascript
_deleteShelf = function (shelfId, callback) {
  var data = {
    'shelf_id': shelfId
  };
  var url = this.endpoint + '/merchant/shelf/del?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_shelf._getAllShelves"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_shelf.</span>_getAllShelves (callback)](#apidoc.element.wechat-api.api_shop_shelf._getAllShelves)
- description and source-code
```javascript
_getAllShelves = function (callback) {
  var url = this.endpoint + '/merchant/shelf/getall?access_token=' + this.token.accessToken;
  this.request(url, {dataType: 'json'}, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_shelf._getShelfById"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_shelf.</span>_getShelfById (shelfId, callback)](#apidoc.element.wechat-api.api_shop_shelf._getShelfById)
- description and source-code
```javascript
_getShelfById = function (shelfId, callback) {
  var data = {
    'shelf_id': shelfId
  };
  var url = this.endpoint + '/merchant/shelf/getbyid?access_token=' + this.token.accessToken;
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_shelf._updateShelf"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_shelf.</span>_updateShelf (shelf, callback)](#apidoc.element.wechat-api.api_shop_shelf._updateShelf)
- description and source-code
```javascript
_updateShelf = function (shelf, callback) {
  var url = this.endpoint + '/merchant/shelf/mod?access_token=' + this.token.accessToken;
  this.request(url, postJSON(shelf), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_shelf.createShelf"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_shelf.</span>createShelf (shelf, callback)](#apidoc.element.wechat-api.api_shop_shelf.createShelf)
- description and source-code
```javascript
createShelf = function (shelf, callback) {
  this.preRequest(this._createShelf, arguments);
}
```
- example usage
```shell
...
var postJSON = util.postJSON;

/**
* 增加货架
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.createShelf(shelf, callback);
* '''
* Shelf:
* '''
* {
*   "shelf_data": {
*     "module_infos": [
*     {
...
```

#### <a name="apidoc.element.wechat-api.api_shop_shelf.deleteShelf"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_shelf.</span>deleteShelf (shelfId, callback)](#apidoc.element.wechat-api.api_shop_shelf.deleteShelf)
- description and source-code
```javascript
deleteShelf = function (shelfId, callback) {
  this.preRequest(this._deleteShelf, arguments);
}
```
- example usage
```shell
...
};

/**
* 删除货架
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.deleteShelf(shelfId, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shop_shelf.getAllShelves"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_shelf.</span>getAllShelves (callback)](#apidoc.element.wechat-api.api_shop_shelf.getAllShelves)
- description and source-code
```javascript
getAllShelves = function (callback) {
  this.preRequest(this._getAllShelves, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_shelf.getShelfById"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_shelf.</span>getShelfById (shelfId, callback)](#apidoc.element.wechat-api.api_shop_shelf.getShelfById)
- description and source-code
```javascript
getShelfById = function (shelfId, callback) {
  this.preRequest(this._getShelfById, arguments);
}
```
- example usage
```shell
...
};

/**
* 根据货架ID获取货架信息
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.getShelfById(shelfId, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_shop_shelf.updateShelf"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_shelf.</span>updateShelf (shelf, callback)](#apidoc.element.wechat-api.api_shop_shelf.updateShelf)
- description and source-code
```javascript
updateShelf = function (shelf, callback) {
  this.preRequest(this._updateShelf, arguments);
}
```
- example usage
```shell
...
};

/**
* 修改货架
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.updateShelf(shelf, callback);
* '''
* Shelf:
* '''
* {
*   "shelf_id": 12345,
*   "shelf_data": ...,
*   "shelf_banner": "http://mmbiz.qpic.cn/mmbiz/ 4whpV1VZl2ibrWQn8zWFUh1YznsMV0XEiavFfLzDWYyvQOBBszXlMaiabGWzz5B2K hNn2IDemHa3iarmCyribYlZYyw
/0",
...
```



# <a name="apidoc.module.wechat-api.api_shop_stock"></a>[module wechat-api.api_shop_stock](#apidoc.module.wechat-api.api_shop_stock)

#### <a name="apidoc.element.wechat-api.api_shop_stock._updateStock"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_stock.</span>_updateStock (number, productId, sku, callback)](#apidoc.element.wechat-api.api_shop_stock._updateStock)
- description and source-code
```javascript
_updateStock = function (number, productId, sku, callback) {
  var url;
  if (number > 0) {
    url = this.endpoint + '/merchant/stock/add?access_token=' + this.token.accessToken;
  } else {
    url = this.endpoint + '/merchant/stock/reduce?access_token=' + this.token.accessToken;
  }
  var data = {
    'product_id': productId,
    'sku_info': sku,
    'quantity': Math.abs(number)
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_shop_stock.updateStock"></a>[function <span class="apidocSignatureSpan">wechat-api.api_shop_stock.</span>updateStock (number, productId, sku, callback)](#apidoc.element.wechat-api.api_shop_stock.updateStock)
- description and source-code
```javascript
updateStock = function (number, productId, sku, callback) {
  this.preRequest(this._updateStock, arguments);
}
```
- example usage
```shell
...
var postJSON = util.postJSON;

/**
* 增加库存
* 详细请看：<http://mp.weixin.qq.com/wiki/8/703923b7349a607f13fb3100163837f0.html>
* Examples:
* '''
* api.updateStock(10, productId, sku, callback); // 增加10件库存
* api.updateStock(-10, productId, sku, callback); // 减少10件库存
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
...
```



# <a name="apidoc.module.wechat-api.api_tag"></a>[module wechat-api.api_tag](#apidoc.module.wechat-api.api_tag)

#### <a name="apidoc.element.wechat-api.api_tag._createTag"></a>[function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>_createTag (name, callback)](#apidoc.element.wechat-api.api_tag._createTag)
- description and source-code
```javascript
_createTag = function (name, callback) {
  // https://api.weixin.qq.com/cgi-bin/tags/create?access_token=ACCESS_TOKEN
  var url = this.endpoint + '/cgi-bin/tags/create?access_token=' + this.token.accessToken;
  var data = {
    'tag': {
      'name': name
    }
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_tag._deleteTag"></a>[function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>_deleteTag (id, callback)](#apidoc.element.wechat-api.api_tag._deleteTag)
- description and source-code
```javascript
_deleteTag = function (id, callback) {
  // http请求方式: POST（请使用https协议）
  // https://api.weixin.qq.com/cgi-bin/tags/delete?access_token=ACCESS_TOKEN
  // POST数据格式：json
  // POST数据例子：{"tag":{"id":108}}
  var url = this.endpoint + '/cgi-bin/tags/delete?access_token=' + this.token.accessToken;
  var data = {
    'tag': {'id': id}
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_tag._editTag"></a>[function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>_editTag (id, name, callback)](#apidoc.element.wechat-api.api_tag._editTag)
- description and source-code
```javascript
_editTag = function (id, name, callback) {
  // https://api.weixin.qq.com/cgi-bin/tags/update?access_token=ACCESS_TOKEN
  // POST数据格式：json
  // POST数据例子：{"tag":{"id":134, "name":"test"}}
  var url = this.endpoint + '/cgi-bin/tags/update?access_token=' + this.token.accessToken;
  var data = {
    'tag': {
      'id': id,
      'name': name
    }
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_tag._getTagUsers"></a>[function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>_getTagUsers (tagId, openid, callback)](#apidoc.element.wechat-api.api_tag._getTagUsers)
- description and source-code
```javascript
_getTagUsers = function (tagId, openid, callback) {
  // http请求方式: POST（请使用https协议）
  // https://api.weixin.qq.com/cgi-bin/user/tag/get?access_token=ACCESS_TOKEN
  // POST数据格式：json
  // POST数据例子：{"tagid":108, "next_openid":"oDF3iYx0ro3_7jD4HFRDfrjdCM58"}
  var url = this.endpoint + '/cgi-bin/user/tag/get?access_token=' + this.token.accessToken;
  var data = {
    'tagid': tagId,
    'next_openid': openid
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_tag._getTags"></a>[function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>_getTags (callback)](#apidoc.element.wechat-api.api_tag._getTags)
- description and source-code
```javascript
_getTags = function (callback) {
  // https://api.weixin.qq.com/cgi-bin/tags/get?access_token=ACCESS_TOKEN
  var url = this.endpoint + '/cgi-bin/tags/get?access_token=' + this.token.accessToken;
  this.request(url, {dataType: 'json'}, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_tag._getUserTags"></a>[function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>_getUserTags (openid, callback)](#apidoc.element.wechat-api.api_tag._getUserTags)
- description and source-code
```javascript
_getUserTags = function (openid, callback) {
  // https://api.weixin.qq.com/cgi-bin/tags/getidlist?access_token=ACCESS_TOKEN
  var url = this.endpoint + '/cgi-bin/tags/getidlist?access_token=' + this.token.accessToken;
  var data = {
    'openid':openid
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_tag._membersBatchtagging"></a>[function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>_membersBatchtagging (tagId, openList, callback)](#apidoc.element.wechat-api.api_tag._membersBatchtagging)
- description and source-code
```javascript
_membersBatchtagging = function (tagId, openList, callback) {
  // https://api.weixin.qq.com/cgi-bin/tags/members/batchtagging?access_token=ACCESS_TOKEN
  var url = this.endpoint + '/cgi-bin/tags/members/batchtagging?access_token=' + this.token.accessToken;
  var data = {
    'openid_list':openList,
    'tagid': tagId
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_tag._membersBatchuntagging"></a>[function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>_membersBatchuntagging (tagId, openList, callback)](#apidoc.element.wechat-api.api_tag._membersBatchuntagging)
- description and source-code
```javascript
_membersBatchuntagging = function (tagId, openList, callback) {
  // https://api.weixin.qq.com/cgi-bin/tags/members/batchuntagging?access_token=ACCESS_TOKEN
  var url = this.endpoint + '/cgi-bin/tags/members/batchuntagging?access_token=' + this.token.accessToken;
  var data = {
    'openid_list':openList,
    'tagid': tagId
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_tag.createTag"></a>[function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>createTag (name, callback)](#apidoc.element.wechat-api.api_tag.createTag)
- description and source-code
```javascript
createTag = function (name, callback) {
  this.preRequest(this._createTag, arguments);
}
```
- example usage
```shell
...
var wrapper = util.wrapper;
var postJSON = util.postJSON;
/**
* 创建标签
* 详情请见：<http://mp.weixin.qq.com/wiki?t=resource/res_main&id=mp1421140837&token=&lang=zh_CN>
* Examples:
* '''
* api.createTag(callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_tag.deleteTag"></a>[function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>deleteTag (id, callback)](#apidoc.element.wechat-api.api_tag.deleteTag)
- description and source-code
```javascript
deleteTag = function (id, callback) {
  this.preRequest(this._deleteTag, arguments);
}
```
- example usage
```shell
...
};

/**
* 删除标签
* 详情请见：<http://mp.weixin.qq.com/wiki?t=resource/res_main&id=mp1421140837&token=&lang=zh_CN>
* Examples:
* '''
* api.deleteTag(id, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_tag.editTag"></a>[function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>editTag (id, name, callback)](#apidoc.element.wechat-api.api_tag.editTag)
- description and source-code
```javascript
editTag = function (id, name, callback) {
  this.preRequest(this._editTag, arguments);
}
```
- example usage
```shell
...
};

/**
* 编辑标签
* 详情请见：<http://mp.weixin.qq.com/wiki?t=resource/res_main&id=mp1421140837&token=&lang=zh_CN>
* Examples:
* '''
* api.editTag(id, name, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_tag.getTagUsers"></a>[function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>getTagUsers (tagId, openid, callback)](#apidoc.element.wechat-api.api_tag.getTagUsers)
- description and source-code
```javascript
getTagUsers = function (tagId, openid, callback) {
  this.preRequest(this._getTagUsers, arguments);
}
```
- example usage
```shell
...
};

/**
* 获取标签下粉丝列表
* 详情请见：<http://mp.weixin.qq.com/wiki?t=resource/res_main&id=mp1421140837&token=&lang=zh_CN>
* Examples:
* '''
* api.getTagUsers(tagid, openid, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_tag.getTags"></a>[function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>getTags (callback)](#apidoc.element.wechat-api.api_tag.getTags)
- description and source-code
```javascript
getTags = function (callback) {
  this.preRequest(this._getTags, arguments);
}
```
- example usage
```shell
...
};

/**
* 获取公众号已创建的标签
* 详情请见：<http://mp.weixin.qq.com/wiki?t=resource/res_main&id=mp1421140837&token=&lang=zh_CN>
* Examples:
* '''
* api.getTags(callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_tag.getUserTags"></a>[function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>getUserTags (openid, callback)](#apidoc.element.wechat-api.api_tag.getUserTags)
- description and source-code
```javascript
getUserTags = function (openid, callback) {
  this.preRequest(this._getUserTags, arguments);
}
```
- example usage
```shell
...
};

/**
* 获取用户身上的标签列表
* 详情请见：<http://mp.weixin.qq.com/wiki?t=resource/res_main&id=mp1421140837&token=&lang=zh_CN>
* Examples:
* '''
* api.getUserTags(openid, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_tag.membersBatchtagging"></a>[function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>membersBatchtagging (tagId, openList, callback)](#apidoc.element.wechat-api.api_tag.membersBatchtagging)
- description and source-code
```javascript
membersBatchtagging = function (tagId, openList, callback) {
  this.preRequest(this._membersBatchtagging, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_tag.membersBatchuntagging"></a>[function <span class="apidocSignatureSpan">wechat-api.api_tag.</span>membersBatchuntagging (tagId, openList, callback)](#apidoc.element.wechat-api.api_tag.membersBatchuntagging)
- description and source-code
```javascript
membersBatchuntagging = function (tagId, openList, callback) {
  this.preRequest(this._membersBatchuntagging, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.wechat-api.api_template"></a>[module wechat-api.api_template](#apidoc.module.wechat-api.api_template)

#### <a name="apidoc.element.wechat-api.api_template._addTemplate"></a>[function <span class="apidocSignatureSpan">wechat-api.api_template.</span>_addTemplate (templateIdShort, callback)](#apidoc.element.wechat-api.api_template._addTemplate)
- description and source-code
```javascript
_addTemplate = function (templateIdShort, callback) {
  var apiUrl = this.endpoint + '/cgi-bin/template/api_add_template?access_token=' + this.token.accessToken;
  var templateId = {
    template_id_short: templateIdShort
  };
  this.request(apiUrl, postJSON(templateId), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_template._delPrivateTemplate"></a>[function <span class="apidocSignatureSpan">wechat-api.api_template.</span>_delPrivateTemplate (templateId, callback)](#apidoc.element.wechat-api.api_template._delPrivateTemplate)
- description and source-code
```javascript
_delPrivateTemplate = function (templateId, callback) {
  var apiUrl = this.endpoint + '/cgi-bin/template/del_private_template?access_token=' + this.token.accessToken;
  var data = {
    template_id: templateId
  };
  this.request(apiUrl, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_template._getAllPrivateTemplate"></a>[function <span class="apidocSignatureSpan">wechat-api.api_template.</span>_getAllPrivateTemplate (callback)](#apidoc.element.wechat-api.api_template._getAllPrivateTemplate)
- description and source-code
```javascript
_getAllPrivateTemplate = function (callback) {
  var apiUrl = this.endpoint + '/cgi-bin/template/get_all_private_template?access_token=' + this.token.accessToken;
  this.request(apiUrl, {dataType: 'json'}, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_template._getIndustry"></a>[function <span class="apidocSignatureSpan">wechat-api.api_template.</span>_getIndustry (callback)](#apidoc.element.wechat-api.api_template._getIndustry)
- description and source-code
```javascript
_getIndustry = function (callback) {
  var apiUrl = this.endpoint + '/cgi-bin/template/get_industry?access_token=' + this.token.accessToken;
  this.request(apiUrl, {dataType: 'json'}, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_template._sendTemplate"></a>[function <span class="apidocSignatureSpan">wechat-api.api_template.</span>_sendTemplate (openid, templateId, url, data, callback, callback2)](#apidoc.element.wechat-api.api_template._sendTemplate)
- description and source-code
```javascript
_sendTemplate = function (openid, templateId, url, data, callback, callback2) {
<span class="apidocCodeCommentSpan">  /*
      duplicated interface 'function (openid, templateId, url, topColor, data, callback)'
   */
</span>  var apiUrl = this.endpoint + '/cgi-bin/message/template/send?access_token=' + this.token.accessToken;

  if (typeof data === 'string') {
    data = callback;
    callback = callback2;
  }

  var template = {
    touser: openid,
    template_id: templateId,
    url: url,
    data: data
  };
  this.request(apiUrl, postJSON(template), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_template._setIndustry"></a>[function <span class="apidocSignatureSpan">wechat-api.api_template.</span>_setIndustry (industryIds, callback)](#apidoc.element.wechat-api.api_template._setIndustry)
- description and source-code
```javascript
_setIndustry = function (industryIds, callback) {
  var apiUrl = this.endpoint + '/cgi-bin/template/api_set_industry?access_token=' + this.token.accessToken;
  this.request(apiUrl, postJSON(industryIds), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_template.addTemplate"></a>[function <span class="apidocSignatureSpan">wechat-api.api_template.</span>addTemplate (templateIdShort, callback)](#apidoc.element.wechat-api.api_template.addTemplate)
- description and source-code
```javascript
addTemplate = function (templateIdShort, callback){
  this.preRequest(this._addTemplate, arguments);
}
```
- example usage
```shell
...
};

/**
* 获得模板ID
* Examples:
* '''
* var templateIdShort = 'TM00015';
* api.addTemplate(templateIdShort, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* @param {String} templateIdShort 模板库中模板的编号，有“TM**”和“OPENTMTM**”等形式
...
```

#### <a name="apidoc.element.wechat-api.api_template.delPrivateTemplate"></a>[function <span class="apidocSignatureSpan">wechat-api.api_template.</span>delPrivateTemplate (templateId, callback)](#apidoc.element.wechat-api.api_template.delPrivateTemplate)
- description and source-code
```javascript
delPrivateTemplate = function (templateId, callback){
  this.preRequest(this._delPrivateTemplate, arguments);
}
```
- example usage
```shell
...
};

/**
* 删除模板
* Examples:
* '''
* var templateId = ”Dyvp3-Ff0cnail_CDSzk1fIc6-9lOkxsQE7exTJbwUE”
* api.delPrivateTemplate(templateId, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* @param {String} templateId 公众帐号下模板消息ID
...
```

#### <a name="apidoc.element.wechat-api.api_template.getAllPrivateTemplate"></a>[function <span class="apidocSignatureSpan">wechat-api.api_template.</span>getAllPrivateTemplate (callback)](#apidoc.element.wechat-api.api_template.getAllPrivateTemplate)
- description and source-code
```javascript
getAllPrivateTemplate = function (callback){
  this.preRequest(this._getAllPrivateTemplate, arguments);
}
```
- example usage
```shell
...
 this.request(apiUrl, postJSON(templateId), wrapper(callback));
};

/**
* 获取模板列表
* Examples:
* '''
* api.getAllPrivateTemplate(callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_template.getIndustry"></a>[function <span class="apidocSignatureSpan">wechat-api.api_template.</span>getIndustry (callback)](#apidoc.element.wechat-api.api_template.getIndustry)
- description and source-code
```javascript
getIndustry = function (callback){
  this.preRequest(this._getIndustry, arguments);
}
```
- example usage
```shell
...
 this.request(apiUrl, postJSON(industryIds), wrapper(callback));
};

/**
* 获取设置的行业信息
* Examples:
* '''
* api.getIndustry(callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* Result:
...
```

#### <a name="apidoc.element.wechat-api.api_template.sendTemplate"></a>[function <span class="apidocSignatureSpan">wechat-api.api_template.</span>sendTemplate (openid, templateId, url, data, callback, callback2)](#apidoc.element.wechat-api.api_template.sendTemplate)
- description and source-code
```javascript
sendTemplate = function (openid, templateId, url, data, callback, callback2) {
  this.preRequest(this._sendTemplate, arguments);
}
```
- example usage
```shell
...
*      "color":"#173177"
*    },
*    "remark":{
*      "value":"欢迎再次购买！",
*      "color":"#173177"
*    }
* };
* api.sendTemplate('openid', templateId, url, data, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* @param {String} openid 用户的openid
...
```

#### <a name="apidoc.element.wechat-api.api_template.setIndustry"></a>[function <span class="apidocSignatureSpan">wechat-api.api_template.</span>setIndustry (industryIds, callback)](#apidoc.element.wechat-api.api_template.setIndustry)
- description and source-code
```javascript
setIndustry = function (industryIds, callback){
  this.preRequest(this._setIndustry, arguments);
}
```
- example usage
```shell
...
* 设置所属行业
* Examples:
* '''
* var industryIds = {
*  "industry_id1":'1',
*  "industry_id2":"4"
* };
* api.setIndustry(industryIds, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* @param {Object} industryIds 公众号模板消息所属行业编号
...
```



# <a name="apidoc.module.wechat-api.api_url"></a>[module wechat-api.api_url](#apidoc.module.wechat-api.api_url)

#### <a name="apidoc.element.wechat-api.api_url._shorturl"></a>[function <span class="apidocSignatureSpan">wechat-api.api_url.</span>_shorturl (longUrl, callback)](#apidoc.element.wechat-api.api_url._shorturl)
- description and source-code
```javascript
_shorturl = function (longUrl, callback) {
  // https://api.weixin.qq.com/cgi-bin/shorturl?access_token=ACCESS_TOKEN
  var url = this.endpoint + '/cgi-bin/shorturl?access_token=' + this.token.accessToken;
  var data = {
    'action': 'long2short',
    'long_url': longUrl
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_url.shorturl"></a>[function <span class="apidocSignatureSpan">wechat-api.api_url.</span>shorturl (longUrl, callback)](#apidoc.element.wechat-api.api_url.shorturl)
- description and source-code
```javascript
shorturl = function (longUrl, callback) {
  this.preRequest(this._shorturl, arguments);
}
```
- example usage
```shell
...
var postJSON = util.postJSON;

/**
* 短网址服务
* 详细细节 http://mp.weixin.qq.com/wiki/10/165c9b15eddcfbd8699ac12b0bd89ae6.html
* Examples:
* '''
* api.shorturl('http://mp.weixin.com', callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
* @param {String} longUrl 需要转换的长链接，支持http://、https://、weixin://wxpay格式的url
...
```



# <a name="apidoc.module.wechat-api.api_user"></a>[module wechat-api.api_user](#apidoc.module.wechat-api.api_user)

#### <a name="apidoc.element.wechat-api.api_user._batchGetUsers"></a>[function <span class="apidocSignatureSpan">wechat-api.api_user.</span>_batchGetUsers (openids, callback)](#apidoc.element.wechat-api.api_user._batchGetUsers)
- description and source-code
```javascript
_batchGetUsers = function (openids, callback) {
  var url = this.endpoint + '/cgi-bin/user/info/batchget?access_token=' + this.token.accessToken;
  var data = {};
  data.user_list = openids.map(function (openid) {
    return {openid: openid, language: 'zh-CN'};
  });
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_user._getFollowers"></a>[function <span class="apidocSignatureSpan">wechat-api.api_user.</span>_getFollowers (nextOpenid, callback)](#apidoc.element.wechat-api.api_user._getFollowers)
- description and source-code
```javascript
_getFollowers = function (nextOpenid, callback) {
  // https://api.weixin.qq.com/cgi-bin/user/get?access_token=ACCESS_TOKEN&next_openid=NEXT_OPENID
  if (typeof nextOpenid === 'function') {
    callback = nextOpenid;
    nextOpenid = '';
  }
  var url = this.endpoint + '/cgi-bin/user/get?next_openid=' + nextOpenid + '&access_token=' + this.token.accessToken;
  this.request(url, {dataType: 'json'}, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_user._getUser"></a>[function <span class="apidocSignatureSpan">wechat-api.api_user.</span>_getUser (options, callback)](#apidoc.element.wechat-api.api_user._getUser)
- description and source-code
```javascript
_getUser = function (options, callback) {
  if (typeof options !== 'object') {
    options = {
      openid: options,
      lang: 'en'
    };
  }
  // https://api.weixin.qq.com/cgi-bin/user/info?access_token=ACCESS_TOKEN&openid=OPENID
  var url = this.endpoint + '/cgi-bin/user/info?openid=' + options.openid + '&lang=' + options.lang + '&access_token=' + this.token
.accessToken;
  this.request(url, {dataType: 'json'}, wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_user._updateRemark"></a>[function <span class="apidocSignatureSpan">wechat-api.api_user.</span>_updateRemark (openid, remark, callback)](#apidoc.element.wechat-api.api_user._updateRemark)
- description and source-code
```javascript
_updateRemark = function (openid, remark, callback) {
  // https://api.weixin.qq.com/cgi-bin/user/info/updateremark?access_token=ACCESS_TOKEN
  var url = this.endpoint + '/cgi-bin/user/info/updateremark?access_token=' + this.token.accessToken;
  var data = {
    openid: openid,
    remark: remark
  };
  this.request(url, postJSON(data), wrapper(callback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_user.batchGetUsers"></a>[function <span class="apidocSignatureSpan">wechat-api.api_user.</span>batchGetUsers (openids, callback)](#apidoc.element.wechat-api.api_user.batchGetUsers)
- description and source-code
```javascript
batchGetUsers = function (openids, callback) {
  this.preRequest(this._batchGetUsers, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.api_user.getFollowers"></a>[function <span class="apidocSignatureSpan">wechat-api.api_user.</span>getFollowers (nextOpenid, callback)](#apidoc.element.wechat-api.api_user.getFollowers)
- description and source-code
```javascript
getFollowers = function (nextOpenid, callback) {
  this.preRequest(this._getFollowers, arguments);
}
```
- example usage
```shell
...
};

/**
* 获取关注者列表
* 详细细节 http://mp.weixin.qq.com/wiki/0/d0e07720fc711c02a3eab6ec33054804.html
* Examples:
* '''
* api.getFollowers(callback);
* // or
* api.getFollowers(nextOpenid, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
...
```

#### <a name="apidoc.element.wechat-api.api_user.getUser"></a>[function <span class="apidocSignatureSpan">wechat-api.api_user.</span>getUser (options, callback)](#apidoc.element.wechat-api.api_user.getUser)
- description and source-code
```javascript
getUser = function (options, callback) {
  this.preRequest(this._getUser, arguments);
}
```
- example usage
```shell
...
var postJSON = util.postJSON;

/**
* 获取用户基本信息。可以设置lang，其中zh_CN 简体，zh_TW 繁体，en 英语。默认为en
* 详情请见：<http://mp.weixin.qq.com/wiki/14/bb5031008f1494a59c6f71fa0f319c66.html>
* Examples:
* '''
* api.getUser(openid, callback);
* api.getUser({openid: 'openid', lang: 'en'}, callback);
* '''
* Callback:
*
* - 'err', 调用失败时得到的异常
* - 'result', 调用正常时得到的对象
*
...
```

#### <a name="apidoc.element.wechat-api.api_user.updateRemark"></a>[function <span class="apidocSignatureSpan">wechat-api.api_user.</span>updateRemark (openid, remark, callback)](#apidoc.element.wechat-api.api_user.updateRemark)
- description and source-code
```javascript
updateRemark = function (openid, remark, callback) {
  this.preRequest(this._updateRemark, arguments);
}
```
- example usage
```shell
...

## Usage

'''js
var WechatAPI = require('wechat-api');

var api = new WechatAPI(appid, appsecret);
api.updateRemark('open_id', 'remarked', function (err, data, res) {
  // TODO
});
'''

### patch()扩展

当微信官方文档已更新，但本库未来得及更新，而又想用新的微信 api 时，可调用 patch 方法来扩展新功能。
...
```



# <a name="apidoc.module.wechat-api.util"></a>[module wechat-api.util](#apidoc.module.wechat-api.util)

#### <a name="apidoc.element.wechat-api.util.make"></a>[function <span class="apidocSignatureSpan">wechat-api.util.</span>make (host, name, fn)](#apidoc.element.wechat-api.util.make)
- description and source-code
```javascript
make = function (host, name, fn) {
  host[name] = function () {
    this.preRequest(this['_' + name], arguments);
  };
  host['_' + name] = fn;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.util.postJSON"></a>[function <span class="apidocSignatureSpan">wechat-api.util.</span>postJSON (data)](#apidoc.element.wechat-api.util.postJSON)
- description and source-code
```javascript
postJSON = function (data) {
  return {
    dataType: 'json',
    type: 'POST',
    data: data,
    headers: {
      'Content-Type': 'application/json'
    }
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wechat-api.util.wrapper"></a>[function <span class="apidocSignatureSpan">wechat-api.util.</span>wrapper (callback)](#apidoc.element.wechat-api.util.wrapper)
- description and source-code
```javascript
wrapper = function (callback) {
  return function (err, data, res) {
    callback = callback || function () {};
    if (err) {
      err.name = 'WeChatAPI' + err.name;
      return callback(err, data, res);
    }
    if (data && data.errcode) {
      err = new Error(data.errmsg);
      err.name = 'WeChatAPIError';
      err.code = data.errcode;
      return callback(err, data, res);
    }
    callback(null, data, res);
  };
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
