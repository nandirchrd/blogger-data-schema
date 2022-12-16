# BLOGGER DATA SCHEMA

## List Data
| No |  Global  |
| -- | -------- |
| 1  | blog     |
| 2  | messages |
| 3  | skin     |
| 4  | template |
| 5  | view     |
| 6  | widget   |
| 7  | widgets  |

| NO | Widgets       |
| -- | ------------- |
| 1  | Adsense       |
| 2  | Attribution   |
| 3  | Blog          |
| 4  | BlogArchive   |
| 5  | BloggerButton |
| 6  | BlogList      |
| 7  | BlogSearch    |
| 8  | ContactForm   |
| 9  | FeaturedPost  |
| 10 | Feed          |
| 11 | Followers     |
| 12 | Header        |
| 13 | HTML/Text     |
| 14 | Image         |
| 15 | Label         |
| 16 | LinkList      |
| 17 | PageList      |
| 18 | PopularPosts  |
| 19 | Profile       |
| 20 | Stats         |
| 21 | Subscribe     |
| 22 | PopularPosts  |
| 23 | Profile       |
| 24 | Stats         |
| 25 | Subscribe     |
| 26 | TextList      |
| 27 | Translate     |
| 28 | Wikipedia     |

## Data Schema
- Global Data
    - blog
        ```typescript
        "data": {
            "blog": {
                "blogId": String,
                "postId": String,
                "pageId": String,
                "title": String,
                "pageTitle": String,
                "pageName": String,
                "searchLabel": String,
                "searchQuery": String,
                "pageType": String,
                "view": String,
                "url": String,
                "canonicalUrl": String,
                "homePageUrl": String,
                "canonicalHomepageUrl": String,
                "searchUrl": String,
                "blogspotFaviconUrl": String,
                "bloggerUrl": String,
                "metaDescription": String,
                "analyticsAccountNumber": String,
                "locale": String,
                "localeUnderscoreDelimited": String,
                "languageDirection": String,
                "encoding": String,
                "hasCustomDomain": Boolean,
                "httpsEnabled": Boolean,
                "enabledCommentProfileImages": Boolean,
                "isPrivate": Boolean,
                "isPrivateBlog": Boolean,
                "adultContent": Boolean,
                "isMobile": Boolean,
                "isMobileRequest": Boolean,
                "mobileClass": String,
                "feedLinks": String,
                "postImageUrl": String,
                "postImageThumbnailUrl": String,
                "latencyHeadScript": String,
                "mobileHeadScript": String,
                "dynamicViewsScriptSrc": String,
                "dynamicViewsCommentsSrc": String,
                "ieCssRetrofitLinks": String,
                "adsenseHostId": String,
                "adsenseClientId": String,
                "adsenseHasAds": Boolean,
                "adsenseAutoAds": Boolean,
                "jumpLinkMessage": String,
                "hasCustomJumpLinkMessage": Boolean,
                "isDynamicViewsAvailable": Boolean,
                "meTag": String,
                "gPlusViewType": String,
                "plusOneApiSrc": String,
                "disableGComments": String,
                "sharing": {
                    "disableGooglePlus": Boolean,
                    "googlePlusBootstrap": String,
                    "googlePlusShareButtonWidth": Number,
                    "platforms": [{
                        "name": String,
                        "key": String,
                        "shareMessage": String,
                        "target": String,
                    }],
                        {
                            "size": Number,
                            "length": Number,
                            "empty": Boolean,
                            "notEmpty": Boolean,
                            "any": Boolean,
                            "first": String,
                            "last": String,
                        }, 
                    ,
                },
            }
        }
        ```
    - view
        ```typescript
        "data": {
            "view": {
                "postId": Number,
                "pageId": Number,
                "type": String,
                "featuredImage": String,
                "title": String,
                "description": String,
                "url": String,
                "isPost": Boolean,
                "isPage": Boolean,
                "isHomepage": Boolean,
                "isSearch": Boolean,
                "isArchive": Boolean,
                "isError": Boolean,
                "isLabelSearch": Boolean,
                "isSingleItem": Boolean,
                "isMultipleItems": Boolean,
                "isMobile": Boolean,
                "isPreview": Boolean,
                "isLayoutMode": Boolean,
                "search": {
                    "resultsMessageHtml": String,
                    "resultsMessage": String,
                    "query": String,
                    "label": String,
                },
                "archive": {
                    "rangeMessage": String,
                    "day": Number,
                    "month": Number,
                    "year": Number,
                },
            }
        }
        ```
- Widgets Data
    - Blog
        ```typescript
        "version 1"
        {
            "title": String,
            "description": String,
            "numPosts": Number,
            "mobile": Boolean,
            "postLabelsLabel": String,
            "timestampLabel": String,
            "authorLabel": String,
            "commentLabel": String,
            "commentLabelPlural": String,
            "postLocationLabel": String,
            "showTimestamp": Boolean,
            "showLocation": Boolean,
            "showAuthor": Boolean,
            "showPostLabels": Boolean,
            "showMobileShare": Boolean,
            "showEmailButton": Boolean,
            "showBlogThisButton": Boolean,
            "showTwitterButton": Boolean,
            "showFacebookButton": Boolean,
            "showPinterestButton": Boolean,
            "showDummy": Boolean,
            "showPlusOne": Boolean,
            "olderPageUrl": String,
            "olderPageTitle": String,
            "newerPageUrl": String,
            "newerPageTitle": String,
            "mobileLinkUrl": String,
            "mobileLinkMsg": String,
            "dekstopLinkUrl": String,
            "dekstopLinkMsg": String,
            "homeMsg": String,
            "navMessage": String,
            "postCommentMsg": String,
            "blogCommentMessage": String,
            "blogTeamBlogMessage": String,
            "feedLinkMsg": String,
            "commentPostedByMsg": String,
            "shareMsg": String,
            "shareToTwitterMsg": String,
            "shareToFacebookMsg": String,
            "shareToPinterestMsg": String,
            "blogThisMsg": String,
            "emailThisMsg": String,
            "emailPostMsg": String,
            "editPostMsg": String,
            "deletCommentMsg": String,
            "adCode": String,
            "cmtIframeInitialHeight": String,
            "showCmtPopup": Boolean,
            "backgroundColor": String,
            "linkColor": String,
            "textColor": String,
            "languageCode": String,
            "feedLinks": [
                {
                    "url": String,
                    "name": String,
                    "feedType": String,
                    "mimeType": String,
                }
            ],
            "posts": [
                {
                    "id": String,
                    "title": String,
                    "body": String,
                    "snippet": String,
                    "longSnippet": String,
                    "url": String,
                    "canonicalUrl": String,
                    "absoluteUrl": String,
                    "link": String,
                    "thumbnailUrl": String,
                    "firstImageUrl": String,
                    "date": date,
                    "dateHeader": String,
                    "timestamp": String,
                    "timestampISO8601": String,
                    "lastUpdatedISO8601": String,
                    "author": String,
                    "authorProfileUrl": String,
                    "authorAboutMe": String,
                    "authorPhoto": {},
                    "hasJumplink": Boolean,
                    "jumpText": String,
                    "isFirstPost": Boolean,
                    "isDateStart": Boolean,
                    "adminClass": String,
                    "editUrl": String,
                    "commentSource": Number,
                    "commentConfig": String,
                    "commentJso": String,
                    "commentMsgs": String,
                    "commentSrc": String,
                    "allowComments": Boolean,
                    "allowNewComments": Boolean,
                    "noNewCommentsText": String,
                    "numComments": Number,
                    "commentLabelFull": String,
                    "addCommentUrl": String,
                    "addCommentOnclick": String,
                    "commentPagingRequired": Boolean,
                    "hadOlderLinks": Boolean,
                    "oldLinkClass": String,
                    "oldestLinkUrl": String,
                    "oldestLinkText": String,
                    "olderLinkUrl": String,
                    "olderLinkText": String,
                    "hasNewerLinks": Boolean,
                    "newLinkClass": String,
                    "newerLinkUrl": String,
                    "newerLinkText": String,
                    "newestLinkUrl": String,
                    "newestLinkText": String,
                    "commentRangeText": String,
                    "commentFromIframeSrc": String,
                    "embedCommentForm": Boolean,
                    "showThreadedComments": Boolean,
                    "commentHtml": String,
                    "avatarIndentClass": String,
                    "includeAd": Boolean,
                    "emailPostUrl": String,
                    "sharePostUrl": String,
                    "dummyTag": String,
                    "googlePlusShareTag": String,
                    "cmtfpIframe": String,
                    "appRpcRelayPath": String,
                    "location": {
                        "mapsUrl": String,
                        "name": String,
                    },
                    "labels": [
                        {
                            "name": String,
                            "url": String,
                            "isLast": String,
                        }
                    ],
                    "feedLinks": [
                        {
                            "url": String,
                            "type": String,
                            "feedType": String,
                            "mimeType": String,
                        }
                    ],
                    "comments": [
                        {
                            "id": String,
                            "inReplyTo": String,
                            "cmtBodyIdPostFix": String,
                            "url": String,
                            "deleteUrl": String,
                            "body": String,
                            "timestamp": String,
                            "timestampValue": Number,
                            "timestampAbs": Number,
                            "author": String,
                            "authorUrl": String,
                            "authorPhoto": {
                                "url": String,
                                "width": Number,
                                "height": Number,
                                "thumbUrl": String,
                                "thumbWidth": Number,
                                "thumbHeight": Number,
                            },
                            "authorAvatarSrc": String,
                            "authorAvatarImage": String,
                            "favicon": String,
                            "anchorName": String,
                            "isDeleted": Boolean,
                            "adminClass": String,
                            "authorClass": String,
                        }
                    ],
                    "enclosures": [],
                }
            ],
        }
        ```

