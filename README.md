# DASH in a Flash Campaign Setup

##### run this sql command

## “DASH in a Flash” patience reward
```
INSERT INTO campaign (
    "id",
    "nameEn",
    "nameTc",
    "descriptionEn",
    "descriptionTc",
    "priority",
    "maxCount",
    "startAt",
    "endAt",
    "campaignMaxCount",
    "discountRules",
    "applicationRules",
    "validityDescriptionEn",
    "validityDescriptionTc",
    "isOnDemand",
    "eventTriggers",
    "sponsorType",
    "availableValue",
    "imageEn",
    "imageTc"
) VALUES (
    'f33c0c00-c7f4-4fb9-bb0a-5f0abd3c7bcf',
    '“DASH in a Flash” patience reward',
    '耐心等閃優惠',
    '$30 off',
    '減 $30',
    '5003',
    '100',
    '2026-02-22 16:00:00',
    '2026-03-06 16:00:00',
    '99999',
    '{
  "if": [
    true,
    -30,
    -30
  ]
}',
'{
  "and": [
    {
      "==": [
        { "var": "transactionType" },
        "TRIP"
      ]
    },
    {
      "==": [
        { "var": "clientType" },
        "DASH"
      ]
    },
    {
      "==": [
        { "var": "platformType" },
        "DASH"
      ]
    },
    {
      "in": [
        { "var": "dayOfWeek" },
        [1, 2, 3, 4, 5]
      ]
    },
    {
      "or": [
        {
          "or": [
            {
              "point_in_polygon": [
                { "var": "origin" },
                [
                  [22.2904036, 114.2079779],
                  [22.287634, 114.2092574],
                  [22.2863385, 114.2100205],
                  [22.2852614, 114.2111376],
                  [22.284765, 114.212704],
                  [22.28477, 114.2152146],
                  [22.284018, 114.2152146],
                  [22.2837065, 114.2158368],
                  [22.2839339, 114.2163116],
                  [22.2842705, 114.2166039],
                  [22.2844731, 114.2171752],
                  [22.2845049, 114.2177237],
                  [22.2850271, 114.2178585],
                  [22.2850846, 114.2190846],
                  [22.2847302, 114.2196992],
                  [22.2852837, 114.2205146],
                  [22.285749, 114.2209008],
                  [22.2871382, 114.2208955],
                  [22.2879817, 114.2209143],
                  [22.2885175, 114.220182],
                  [22.2881304, 114.2169849],
                  [22.2882445, 114.2138199],
                  [22.2894333, 114.2140237],
                  [22.2905687, 114.2123285],
                  [22.2923643, 114.209716],
                  [22.2914088, 114.2083454],
                  [22.2904036, 114.2079779]
                ]
              ]
            },
            {
              "point_in_polygon": [
                { "var": "origin" },
                [
                  [22.2907235, 114.2084467],
                  [22.2912099, 114.208613],
                  [22.2921831, 114.2100218],
                  [22.2927288, 114.2086774],
                  [22.293642, 114.2049116],
                  [22.2938431, 114.2025164],
                  [22.2923516, 114.202857],
                  [22.291535, 114.2030743],
                  [22.291813, 114.2043886],
                  [22.2914184, 114.2046165],
                  [22.2909444, 114.2047345],
                  [22.2909618, 114.2053059],
                  [22.2908278, 114.2063264],
                  [22.290386, 114.2075341],
                  [22.2901465, 114.2079661],
                  [22.2899368, 114.2081728],
                  [22.2907235, 114.2084467]
                ]
              ]
            },
            {
              "point_in_polygon": [
                { "var": "origin" },
                [
                  [22.289514, 114.1913723],
                  [22.2878065, 114.1936361],
                  [22.2899408, 114.1954385],
                  [22.291535, 114.2030743],
                  [22.2938431, 114.2025164],
                  [22.2917377, 114.1937112],
                  [22.289514, 114.1913723]
                ]
              ]
            }
          ]
        },
        {
          "or": [
            {
              "point_in_polygon": [
                { "var": "destination" },
                [
                  [22.2904036, 114.2079779],
                  [22.287634, 114.2092574],
                  [22.2863385, 114.2100205],
                  [22.2852614, 114.2111376],
                  [22.284765, 114.212704],
                  [22.28477, 114.2152146],
                  [22.284018, 114.2152146],
                  [22.2837065, 114.2158368],
                  [22.2839339, 114.2163116],
                  [22.2842705, 114.2166039],
                  [22.2844731, 114.2171752],
                  [22.2845049, 114.2177237],
                  [22.2850271, 114.2178585],
                  [22.2850846, 114.2190846],
                  [22.2847302, 114.2196992],
                  [22.2852837, 114.2205146],
                  [22.285749, 114.2209008],
                  [22.2871382, 114.2208955],
                  [22.2879817, 114.2209143],
                  [22.2885175, 114.220182],
                  [22.2881304, 114.2169849],
                  [22.2882445, 114.2138199],
                  [22.2894333, 114.2140237],
                  [22.2905687, 114.2123285],
                  [22.2923643, 114.209716],
                  [22.2914088, 114.2083454],
                  [22.2904036, 114.2079779]
                ]
              ]
            },
            {
              "point_in_polygon": [
                { "var": "destination" },
                [
                  [22.2907235, 114.2084467],
                  [22.2912099, 114.208613],
                  [22.2921831, 114.2100218],
                  [22.2927288, 114.2086774],
                  [22.293642, 114.2049116],
                  [22.2938431, 114.2025164],
                  [22.2923516, 114.202857],
                  [22.291535, 114.2030743],
                  [22.291813, 114.2043886],
                  [22.2914184, 114.2046165],
                  [22.2909444, 114.2047345],
                  [22.2909618, 114.2053059],
                  [22.2908278, 114.2063264],
                  [22.290386, 114.2075341],
                  [22.2901465, 114.2079661],
                  [22.2899368, 114.2081728],
                  [22.2907235, 114.2084467]
                ]
              ]
            },
            {
              "point_in_polygon": [
                { "var": "destination" },
                [
                  [22.289514, 114.1913723],
                  [22.2878065, 114.1936361],
                  [22.2899408, 114.1954385],
                  [22.291535, 114.2030743],
                  [22.2938431, 114.2025164],
                  [22.2917377, 114.1937112],
                  [22.289514, 114.1913723]
                ]
              ]
            }
          ]
        }
      ]
    }
  ]
}',
'Any ride on a meter taxi to/from Quarry Bay or Tai Koo on weekdays',
'任何平日往返鰂魚涌或北角之咪錶的士行程',
'false',
'{
"1. User submitted the order on weekdays from February 23rd to March 6th, AND",
"2. User selected a pick-up or drop-off location in our designated Quarry Bay and Tai Koo area, AND",
"3. User waited for more than 47 seconds to match with a driver, AND",
"4. User completed the trip"
}',
'DASH',
'30',
'https://www.d-ash.com/',
'https://www.d-ash.com/'
)
```

## “DASH in a Flash” experience reward
```
INSERT INTO campaign (
    "id",
    "nameEn",
    "nameTc",
    "descriptionEn",
    "descriptionTc",
    "priority",
    "maxCount",
    "startAt",
    "endAt",
    "campaignMaxCount",
    "discountRules",
    "applicationRules",
    "validityDescriptionEn",
    "validityDescriptionTc",
    "isOnDemand",
    "sponsorType",
    "availableValue",
    "imageEn",
    "imageTc"
) VALUES (
    '40d0c906-e621-4d56-8ee9-7d66fd9c7376',
    '“DASH in a Flash” experience reward',
    '快閃體驗優惠',
    '$15 off',
    '減 $15',
    '5002',
    '2',
    '2026-02-22 16:00:00',
    '2026-03-06 16:00:00',
    '99999',
    '{
  "if": [
    true,
    -15,
    -15
  ]
}',
'{
  "and": [
    {
      "==": [
        { "var": "transactionType" },
        "TRIP"
      ]
    },
    {
      "==": [
        { "var": "clientType" },
        "DASH"
      ]
    },
    {
      "==": [
        { "var": "platformType" },
        "DASH"
      ]
    },
    {
      "in": [
        { "var": "dayOfWeek" },
        [1, 2, 3, 4, 5]
      ]
    },
    {
      "or": [
        {
          "or": [
            {
              "point_in_polygon": [
                { "var": "origin" },
                [
                  [22.2904036, 114.2079779],
                  [22.287634, 114.2092574],
                  [22.2863385, 114.2100205],
                  [22.2852614, 114.2111376],
                  [22.284765, 114.212704],
                  [22.28477, 114.2152146],
                  [22.284018, 114.2152146],
                  [22.2837065, 114.2158368],
                  [22.2839339, 114.2163116],
                  [22.2842705, 114.2166039],
                  [22.2844731, 114.2171752],
                  [22.2845049, 114.2177237],
                  [22.2850271, 114.2178585],
                  [22.2850846, 114.2190846],
                  [22.2847302, 114.2196992],
                  [22.2852837, 114.2205146],
                  [22.285749, 114.2209008],
                  [22.2871382, 114.2208955],
                  [22.2879817, 114.2209143],
                  [22.2885175, 114.220182],
                  [22.2881304, 114.2169849],
                  [22.2882445, 114.2138199],
                  [22.2894333, 114.2140237],
                  [22.2905687, 114.2123285],
                  [22.2923643, 114.209716],
                  [22.2914088, 114.2083454],
                  [22.2904036, 114.2079779]
                ]
              ]
            },
            {
              "point_in_polygon": [
                { "var": "origin" },
                [
                  [22.2907235, 114.2084467],
                  [22.2912099, 114.208613],
                  [22.2921831, 114.2100218],
                  [22.2927288, 114.2086774],
                  [22.293642, 114.2049116],
                  [22.2938431, 114.2025164],
                  [22.2923516, 114.202857],
                  [22.291535, 114.2030743],
                  [22.291813, 114.2043886],
                  [22.2914184, 114.2046165],
                  [22.2909444, 114.2047345],
                  [22.2909618, 114.2053059],
                  [22.2908278, 114.2063264],
                  [22.290386, 114.2075341],
                  [22.2901465, 114.2079661],
                  [22.2899368, 114.2081728],
                  [22.2907235, 114.2084467]
                ]
              ]
            },
            {
              "point_in_polygon": [
                { "var": "origin" },
                [
                  [22.289514, 114.1913723],
                  [22.2878065, 114.1936361],
                  [22.2899408, 114.1954385],
                  [22.291535, 114.2030743],
                  [22.2938431, 114.2025164],
                  [22.2917377, 114.1937112],
                  [22.289514, 114.1913723]
                ]
              ]
            }
          ]
        },
        {
          "or": [
            {
              "point_in_polygon": [
                { "var": "destination" },
                [
                  [22.2904036, 114.2079779],
                  [22.287634, 114.2092574],
                  [22.2863385, 114.2100205],
                  [22.2852614, 114.2111376],
                  [22.284765, 114.212704],
                  [22.28477, 114.2152146],
                  [22.284018, 114.2152146],
                  [22.2837065, 114.2158368],
                  [22.2839339, 114.2163116],
                  [22.2842705, 114.2166039],
                  [22.2844731, 114.2171752],
                  [22.2845049, 114.2177237],
                  [22.2850271, 114.2178585],
                  [22.2850846, 114.2190846],
                  [22.2847302, 114.2196992],
                  [22.2852837, 114.2205146],
                  [22.285749, 114.2209008],
                  [22.2871382, 114.2208955],
                  [22.2879817, 114.2209143],
                  [22.2885175, 114.220182],
                  [22.2881304, 114.2169849],
                  [22.2882445, 114.2138199],
                  [22.2894333, 114.2140237],
                  [22.2905687, 114.2123285],
                  [22.2923643, 114.209716],
                  [22.2914088, 114.2083454],
                  [22.2904036, 114.2079779]
                ]
              ]
            },
            {
              "point_in_polygon": [
                { "var": "destination" },
                [
                  [22.2907235, 114.2084467],
                  [22.2912099, 114.208613],
                  [22.2921831, 114.2100218],
                  [22.2927288, 114.2086774],
                  [22.293642, 114.2049116],
                  [22.2938431, 114.2025164],
                  [22.2923516, 114.202857],
                  [22.291535, 114.2030743],
                  [22.291813, 114.2043886],
                  [22.2914184, 114.2046165],
                  [22.2909444, 114.2047345],
                  [22.2909618, 114.2053059],
                  [22.2908278, 114.2063264],
                  [22.290386, 114.2075341],
                  [22.2901465, 114.2079661],
                  [22.2899368, 114.2081728],
                  [22.2907235, 114.2084467]
                ]
              ]
            },
            {
              "point_in_polygon": [
                { "var": "destination" },
                [
                  [22.289514, 114.1913723],
                  [22.2878065, 114.1936361],
                  [22.2899408, 114.1954385],
                  [22.291535, 114.2030743],
                  [22.2938431, 114.2025164],
                  [22.2917377, 114.1937112],
                  [22.289514, 114.1913723]
                ]
              ]
            }
          ]
        }
      ]
    }
  ]
}',
'Any ride on a meter taxi to/from Quarry Bay or Tai Koo on weekdays',
'任何平日往返鰂魚涌或北角之咪錶的士行程',
'false',
'DASH',
'15',
'https://www.d-ash.com/',
'https://www.d-ash.com/'
)
```
## “DASH in a Flash” challenge reward
```
INSERT INTO campaign (
    "id",
    "nameEn",
    "nameTc",
    "descriptionEn",
    "descriptionTc",
    "priority",
    "maxCount",
    "startAt",
    "endAt",
    "campaignMaxCount",
    "discountRules",
    "applicationRules",
    "validityDescriptionEn",
    "validityDescriptionTc",
    "isOnDemand",
    "eventTriggers",
    "sponsorType",
    "availableValue",
    "imageEn",
    "imageTc"
) VALUES (
    'ed9a1180-b168-45ff-9f2b-d426126aec7b',
    '“DASH in a Flash” challenge reward',
    '快閃王優惠',
    '$50 off',
    '減 $50',
    '5000',
    '1',
    '2026-02-22 16:00:00',
    '2026-04-05 16:00:00',
    '99999',
    '{
  "if": [
    true,
    -50,
    -50
  ]
}',
'{
  "and": [
    { "==": [ { "var": "clientType" }, "DASH" ] },
    { "==": [ { "var": "platformType" }, "DASH" ] },
    { "==": [ { "var": "transactionType" }, "TRIP" ] },
    { "in": [ { "var": "dayOfWeek" }, [1,2,3,4,5] ] },
    {
      "or": [
        {
          "or": [
            {
              "point_in_polygon": [
                { "var": "origin" },
                [
                  [22.2904036, 114.2079779],
                  [22.287634, 114.2092574],
                  [22.2863385, 114.2100205],
                  [22.2852614, 114.2111376],
                  [22.284765, 114.212704],
                  [22.28477, 114.2152146],
                  [22.284018, 114.2152146],
                  [22.2837065, 114.2158368],
                  [22.2839339, 114.2163116],
                  [22.2842705, 114.2166039],
                  [22.2844731, 114.2171752],
                  [22.2845049, 114.2177237],
                  [22.2850271, 114.2178585],
                  [22.2850846, 114.2190846],
                  [22.2847302, 114.2196992],
                  [22.2852837, 114.2205146],
                  [22.285749, 114.2209008],
                  [22.2871382, 114.2208955],
                  [22.2879817, 114.2209143],
                  [22.2885175, 114.220182],
                  [22.2881304, 114.2169849],
                  [22.2882445, 114.2138199],
                  [22.2894333, 114.2140237],
                  [22.2905687, 114.2123285],
                  [22.2923643, 114.209716],
                  [22.2914088, 114.2083454],
                  [22.2904036, 114.2079779]
                ]
              ]
            },
            {
              "point_in_polygon": [
                { "var": "origin" },
                [
                  [22.2907235, 114.2084467],
                  [22.2912099, 114.208613],
                  [22.2921831, 114.2100218],
                  [22.2927288, 114.2086774],
                  [22.293642, 114.2049116],
                  [22.2938431, 114.2025164],
                  [22.2923516, 114.202857],
                  [22.291535, 114.2030743],
                  [22.291813, 114.2043886],
                  [22.2914184, 114.2046165],
                  [22.2909444, 114.2047345],
                  [22.2909618, 114.2053059],
                  [22.2908278, 114.2063264],
                  [22.290386, 114.2075341],
                  [22.2901465, 114.2079661],
                  [22.2899368, 114.2081728],
                  [22.2907235, 114.2084467]
                ]
              ]
            },
            {
              "point_in_polygon": [
                { "var": "origin" },
                [
                  [22.289514, 114.1913723],
                  [22.2878065, 114.1936361],
                  [22.2899408, 114.1954385],
                  [22.291535, 114.2030743],
                  [22.2938431, 114.2025164],
                  [22.2917377, 114.1937112],
                  [22.289514, 114.1913723]
                ]
              ]
            }
          ]
        },
        {
          "or": [
            {
              "point_in_polygon": [
                { "var": "destination" },
                [
                  [22.2904036, 114.2079779],
                  [22.287634, 114.2092574],
                  [22.2863385, 114.2100205],
                  [22.2852614, 114.2111376],
                  [22.284765, 114.212704],
                  [22.28477, 114.2152146],
                  [22.284018, 114.2152146],
                  [22.2837065, 114.2158368],
                  [22.2839339, 114.2163116],
                  [22.2842705, 114.2166039],
                  [22.2844731, 114.2171752],
                  [22.2845049, 114.2177237],
                  [22.2850271, 114.2178585],
                  [22.2850846, 114.2190846],
                  [22.2847302, 114.2196992],
                  [22.2852837, 114.2205146],
                  [22.285749, 114.2209008],
                  [22.2871382, 114.2208955],
                  [22.2879817, 114.2209143],
                  [22.2885175, 114.220182],
                  [22.2881304, 114.2169849],
                  [22.2882445, 114.2138199],
                  [22.2894333, 114.2140237],
                  [22.2905687, 114.2123285],
                  [22.2923643, 114.209716],
                  [22.2914088, 114.2083454],
                  [22.2904036, 114.2079779]
                ]
              ]
            },
            {
              "point_in_polygon": [
                { "var": "destination" },
                [
                  [22.2907235, 114.2084467],
                  [22.2912099, 114.208613],
                  [22.2921831, 114.2100218],
                  [22.2927288, 114.2086774],
                  [22.293642, 114.2049116],
                  [22.2938431, 114.2025164],
                  [22.2923516, 114.202857],
                  [22.291535, 114.2030743],
                  [22.291813, 114.2043886],
                  [22.2914184, 114.2046165],
                  [22.2909444, 114.2047345],
                  [22.2909618, 114.2053059],
                  [22.2908278, 114.2063264],
                  [22.290386, 114.2075341],
                  [22.2901465, 114.2079661],
                  [22.2899368, 114.2081728],
                  [22.2907235, 114.2084467]
                ]
              ]
            },
            {
              "point_in_polygon": [
                { "var": "destination" },
                [
                  [22.289514, 114.1913723],
                  [22.2878065, 114.1936361],
                  [22.2899408, 114.1954385],
                  [22.291535, 114.2030743],
                  [22.2938431, 114.2025164],
                  [22.2917377, 114.1937112],
                  [22.289514, 114.1913723]
                ]
              ]
            }
          ]
        }
      ]
    }
  ]
}',
'Any ride on a meter taxi',
'任何咪錶的士行程',
'false',
'{
"1. User completed three trips on weekdays from February 23rd to March 6th, AND",
"2. User selected a pick-up OR drop-off location in our designated Quarry Bay and Tai Koo area for all three orders"
}',
'DASH',
'50',
'https://www.d-ash.com/',
'https://www.d-ash.com/'
)
```

##### n8n set-up:
### Global Modules:
-  https://workflows.qa.dash-hk.com/workflow/aeObrO3eL0Ib9CgJ 
    - update this workflow to cater the destination lat & lng
- https://workflows.qa.dash-hk.com/workflow/P204M8985d7Rdn7T
    - worklow that handles the sending of push notif or inbox message
- https://workflows.qa.dash-hk.com/workflow/JWsqGORIaDUMFE3X
    - workflow that responsible for setting up the discount to the user

### DASH-3064 Modules:
- https://workflows.qa.dash-hk.com/workflow/lIDFTLpxt5Stp5JZ
    - this module is responsible for setting up the needed params ( i18n, banner, etc... )
- https://workflows.qa.dash-hk.com/workflow/hciVgz5NiJhnroxK
    - this module is used to prepare the needed layout of the dialog that would be send to the user if no driver accepted ( remind user to keep waiting )
- https://workflows.qa.dash-hk.com/workflow/Fs0FjF7cV0ixYjbq
    - this module is used to prepare the needed msg to be display ( if app is on foreground or in background )

### DASH-3064:
- https://workflows.qa.dash-hk.com/workflow/53zvvTbyUxcC2BCX
    - this workflow is responsible for the default banner display of the user

### DASH-3064 Triggers:
- https://workflows.qa.dash-hk.com/workflow/9zJ5s2sjQbhc8fRx
    - trigger when the driver accepted the order
- https://workflows.qa.dash-hk.com/workflow/Z3YxWM4rGPYawzwm
    - this trigger help to identify if needed to remind the user or not
- https://workflows.qa.dash-hk.com/workflow/jPtVkjqP4rIbalUk
    - this trigger when order change to pending and it remind the user
- https://workflows.qa.dash-hk.com/workflow/7BlcsYWkggLyNPQW
    - this trigger for the second and third follow-up reminders ( this call the module '[module] Patience after time snack bar' which is responsible for the neede msg to display ( app is on foreground or in background )
- https://workflows.qa.dash-hk.com/workflow/UoMJbJpaw50mkBDu
    - this trigger when trip end ( also responsible for issuing a campaign discount and sending notification )

### DASH-3286 Modules:
- https://workflows.qa.dash-hk.com/workflow/SHI32OqvbMwcoSFXqbgJ7
    - this module is responsible for setting up the polygons of the "Quarry Bay", "Quarry Bay / Taikoo CBD", and "North Point"
- https://workflows.qa.dash-hk.com/workflow/QelFyPtbg8QBLy4W
    - this module is responsible for setting up the neede params ( origin lat/lng and destination lat/lng )
- https://workflows.qa.dash-hk.com/workflow/M0CCT4ws8DlGzylT
    - this module check if the given params are within the defined campaign area

### DASH-3286 Triggers:
- https://workflows.qa.dash-hk.com/workflow/ZSBoP0vv0h5MxWg
    - responsible for the updating the banner to be display based on the total trips within the campaign area 
