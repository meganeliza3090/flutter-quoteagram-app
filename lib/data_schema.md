# Data Schema Document

## Collections:

1. ### Users

## User Model

{
    id: Auto-generated,
    userName: String,
    firstName: String,
    lastName: String,
    email: String,
    profileImage: String,
    friends: [
        userId,
        userId
    ],
    quotes: [
      quoteImgAndText[
        quoteImg: String,
        quoteText: String,
      ],
      quoteImgAndText[
        quoteImg: String,
        quoteText: String,
      ]  
    ],
    sentQuotes: [
      sentQuote [
        sentQuoteImg: String,
        SentQuoteText: String,
      ],
      sentQuote [
        sentQuoteImg: String,
        sentQuoteText: String,
      ]  
    ]
}

## User Object Example
{
    id: aggghafhr5agrsghw19i,
    userName: meganeliza3090,
    firstName: Megan,
    lastName: O'Brien,
    profileImage:  https://profileImg.jpeg,
    friends: [
        ghhae1rahr2ah5,
        rhaerhr9421har,
    ],
    savedQuotes: [
      saveQuote [
        saveQuoteImg: https://quoteImg.jpeg,
        saveQuoteText: "Quote text here",
      ],
      saveQuote [
        saveQuoteImg: https://quoteImg.jpeg,
        saveQuoteText: "Quote text here",
      ]  
    ],
    sentQuotes: [
      sentQuote [
        sentQuoteImg: https://quoteImg.jpeg,
        SentQuoteText: "Quote text here",
      ],
      sentQuote [
        sentQuoteImg: https://quoteImg.jpeg,
        sentQuoteText: "Quote text here",
      ]  
    ]
}

2. ### Saved Quotes

## Save Quotes Model
{
    id: Auto-generated,
    date: String,
    fromUserId: String,
    quotes: [
        quote: [
            quoteImg: String,
            quoteText: String,
        ]
    ]
}

## Save Quotes Example
{
    id: gddhaer45haerhigw,
    date: 03-25-21,
    toUserId: sfjarehjreahrrt,
    quotes: [
        quote: [
            quoteImg: https://quoteImg.jpeg,
            quoteText: "Quote here",
        ]
        quote: [
            quoteImg: https://quoteImg.jpeg,
            quoteText: "Quote here",
        ]
    ]
}




3. ### Sent Quotes

## Sent Quotes Model
{
    id: Auto-generated,
    date: String,
    toUserId: String,
    quotes: [
        quote: [
            quoteImg: https://quoteImg.jpeg,
            quoteText: "Quote here",
        ]
        quote: [
            quoteImg: https://quoteImg.jpeg,
            quoteText: "Quote here",
        ]
    ]
}

## Sent Object Example
{
    id: herhrjtrk49ah1rah4,
    date: 01-05-21,
    toUserId: sfjterj81rhajrt,
    quotes: [
        quote: [
            quoteImg: https://quoteImg.jpeg,
            quoteText: "Quote here",
        ]
        quote: [
            quoteImg: https://quoteImg.jpeg,
            quoteText: "Quote here",
        ]
    ]
}