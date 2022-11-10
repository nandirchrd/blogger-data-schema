# BLOGGER DATA SCHEMA

## List Data
- Global
    - blog
    - messages
    - skin
    - template
    - view
    - widget
    - widgets
- Widgets
    - Adsense
    - Attribution
    - Blog
    - BlogArchive
    - BloggerButton
    - BlogList
    - BlogSearch
    - ContactForm
    - FeaturedPost
    - Feed
    - Followers
    - Header
    - HTML/Text
    - Image
    - Label
    - LinkList
    - PageList
    - PopularPosts
    - Profile
    - Stats
    - Subscribe
    - TextList
    - Translate
    - Wikipedia

## Data Schema
- Global Data
    - blog
        ```json
        "data": {
            "blog": {
                "blogId": string,
                "postId": string,
                "pageId": string,
                "title": string,
                "pageTitle": string,
                "pageName": string,
                "searchLabel": string,
                "searchQuery": string,
                "pageType": string,
                "view": string,
                "url": string,
                "canonicalUrl": string,
                "homePageUrl": string,
                "canonicalHomepageUrl": string,
                "searchUrl": string,
                "blogspotFaviconUrl": string,
                "bloggerUrl": string,
                "metaDescription": string,
                "analyticsAccountNumber": string,
                "locale": string,
                "localeUnderscoreDelimited": string,
                "languageDirection": string,
                "encoding": string,
                "hasCustomDomain": boolean,
                "httpsEnabled": boolean,
                "enabledCommentProfileImages": boolean,
                "isPrivate": boolean,
                "isPrivateBlog": boolean,
                "adultContent": boolean,
                "isMobile": boolean,
                "isMobileRequest": boolean,
                "mobileClass": string,
                "feedLinks": string,
                "postImageUrl": string,
                "postImageThumbnailUrl": string,
                "latencyHeadScript": string,
                "mobileHeadScript": string,
                "dynamicViewsScriptSrc": string,
                "dynamicViewsCommentsSrc": string,
                "ieCssRetrofitLinks": string,
                "adsenseHostId": string,
                "adsenseClientId": string,
                "adsenseHasAds": boolean,
                "adsenseAutoAds": boolean,
                "jumpLinkMessage": string,
                "hasCustomJumpLinkMessage": boolean,
                "isDynamicViewsAvailable": boolean,
                "meTag": string,
                "gPlusViewType": string,
                "plusOneApiSrc": string,
                "disableGComments": string,
                "sharing": {
                    "disableGooglePlus": boolean,
                    "googlePlusBootstrap": string,
                    "googlePlusShareButtonWidth": number,
                    "platforms": [{
                        "name": string,
                        "key": string,
                        "shareMessage": string,
                        "target": string,
                    }],
                        {
                            "size": number,
                            "length": number,
                            "empty": boolean,
                            "notEmpty": boolean,
                            "any": boolean,
                            "first": string,
                            "last": string,
                        }, 
                    ,
                },
            }
        }
        ```
    - view
    ```json
        "data": {
            "view": {
                "postId": number,
                "pageId": number,
                "type": string,
                "featuredImage": string,
                "title": string,
                "description": string,
                "url": string,
                "isPost": boolean,
                "isPage": boolean,
                "isHomepage": boolean,
                "isSearch": boolean,
                "isArchive": boolean,
                "isError": boolean,
                "isLabelSearch": boolean,
                "isSingleItem": boolean,
                "isMultipleItems": boolean,
                "isMobile": boolean,
                "isPreview": boolean,
                "isLayoutMode": boolean,
                "search": {
                    "resultsMessageHtml": string,
                    "resultsMessage": string,
                    "query": string,
                    "label": string,
                },
                "archive": {
                    "rangeMessage": string,
                    "day": number,
                    "month": number,
                    "year": number,
                },
            }
        }
- Widgets Data
    - Blog
    ```json
        "version 1"
        {
            "title": string,
            "description": string,
            "numPosts": number,
            "mobile": boolean,
            "postLabelsLabel": string,
            "timestampLabel": string,
            "authorLabel": string,
            "commentLabel": string,
            "commentLabelPlural": string,
            "postLocationLabel": string,
            "showTimestamp": boolean,
            "showLocation": boolean,
            "showAuthor": boolean,
            "showPostLabels": boolean,
            "showMobileShare": boolean,
            "showEmailButton": boolean,
            "showBlogThisButton": boolean,
            "showTwitterButton": boolean,
            "showFacebookButton": boolean,
            "showPinterestButton": boolean,
            "showDummy": boolean,
            "showPlusOne": boolean,
            "olderPageUrl": string,
            "olderPageTitle": string,
            "newerPageUrl": string,
            "newerPageTitle": string,
            "mobileLinkUrl": string,
            "mobileLinkMsg": string,
            "dekstopLinkUrl": string,
            "dekstopLinkMsg": string,
            "homeMsg": string,
            "navMessage": string,
            "postCommentMsg": string,
            "blogCommentMessage": string,
            "blogTeamBlogMessage": string,
            "feedLinkMsg": string,
            "commentPostedByMsg": string,
            "shareMsg": string,
            "shareToTwitterMsg": string,
            "shareToFacebookMsg": string,
            "shareToPinterestMsg": string,
            "blogThisMsg": string,
            "emailThisMsg": string,
            "emailPostMsg": string,
            "editPostMsg": string,
            "deletCommentMsg": string,
            "adCode": string,
            "cmtIframeInitialHeight": string,
            "showCmtPopup": boolean,
            "backgroundColor": string,
            "linkColor": string,
            "textColor": string,
            "languageCode": string,
            "feedLinks": [
                {
                    "url": string,
                    "name": string,
                    "feedType": string,
                    "mimeType": string,
                }
            ],
            "posts": [
                {
                    "id": string,
                    "title": string,
                    "body": string,
                    "snippet": string,
                    "longSnippet": string,
                    "url": string,
                    "canonicalUrl": string,
                    "absoluteUrl": string,
                    "link": string,
                    "thumbnailUrl": string,
                    "firstImageUrl": string,
                    "date": date,
                    "dateHeader": string,
                    "timestamp": string,
                    "timestampISO8601": string,
                    "lastUpdatedISO8601": string,
                    "author": string,
                    "authorProfileUrl": string,
                    "authorAboutMe": string,
                    "authorPhoto": {},
                    "hasJumplink": boolean,
                    "jumpText": string,
                    "isFirstPost": boolean,
                    "isDateStart": boolean,
                    "adminClass": string,
                    "editUrl": string,
                    "commentSource": number,
                    "commentConfig": string,
                    "commentJso": string,
                    "commentMsgs": string,
                    "commentSrc": string,
                    "allowComments": boolean,
                    "allowNewComments": boolean,
                    "noNewCommentsText": string,
                    "numComments": number,
                    "commentLabelFull": string,
                    "addCommentUrl": string,
                    "addCommentOnclick": string,
                    "commentPagingRequired": boolean,
                    "hadOlderLinks": boolean,
                    "oldLinkClass": string,
                    "oldestLinkUrl": string,
                    "oldestLinkText": string,
                    "olderLinkUrl": string,
                    "olderLinkText": string,
                    "hasNewerLinks": boolean,
                    "newLinkClass": string,
                    "newerLinkUrl": string,
                    "newerLinkText": string,
                    "newestLinkUrl": string,
                    "newestLinkText": string,
                    "commentRangeText": string,
                    "commentFromIframeSrc": string,
                    "embedCommentForm": boolean,
                    "showThreadedComments": boolean,
                    "commentHtml": string,
                    "avatarIndentClass": string,
                    "includeAd": boolean,
                    "emailPostUrl": string,
                    "sharePostUrl": string,
                    "dummyTag": string,
                    "googlePlusShareTag": string,
                    "cmtfpIframe": string,
                    "appRpcRelayPath": string,
                    "location": {
                        "mapsUrl": string,
                        "name": string,
                    },
                    "labels": [
                        {
                            "name": string,
                            "url": string,
                            "isLast": string,
                        }
                    ],
                    "feedLinks": [
                        {
                            "url": string,
                            "type": string,
                            "feedType": string,
                            "mimeType": string,
                        }
                    ],
                    "comments": [
                        {
                            "id": string,
                            "inReplyTo": string,
                            "cmtBodyIdPostFix": string,
                            "url": string,
                            "deleteUrl": string,
                            "body": string,
                            "timestamp": string,
                            "timestampValue": number,
                            "timestampAbs": number,
                            "author": string,
                            "authorUrl": string,
                            "authorPhoto": {
                                "url": string,
                                "width": number,
                                "height": number,
                                "thumbUrl": string,
                                "thumbWidth": number,
                                "thumbHeight": number,
                            },
                            "authorAvatarSrc": string,
                            "authorAvatarImage": string,
                            "favicon": string,
                            "anchorName": string,
                            "isDeleted": boolean,
                            "adminClass": string,
                            "authorClass": string,
                        }
                    ],
                    "enclosures": [],
                }
            ],
        }

        "version 2"
        {
            "title": string,
            "title": string,
            "title": string,
            "title": string,
            "title": string,
            "title": string,
            "title": string,
            "title": string,
            "title": string,
            "title": string,
            "title": string,
            "title": string,
            "title": string,
            "title": string,
            "title": string,
            "title": string,
            "title": string,
            "title": string,
        }
    ```

