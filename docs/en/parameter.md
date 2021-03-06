# Parameters

::: tip

All parameters can be linked with `&` to used together to generate a complex feed

:::

## Filtering

The following URL query parameters are supported, Regex support is built-in

Set `filter` to include the content

-   filter: filter title and description

-   filter_title: filter title only

-   filter_description: filter description only

-   filter_author: filter author only

-   filter_time: filter pubDate, value for second number, return specified time range. Item without `pubDate` will not be filtered.

For example: [https://rsshub.app/dribbble/popular?filter=Blue|Yellow|Black](https://rsshub.app/dribbble/popular?filter=Blue|Yellow|Black)

Set `filterout` to exclude unwanted content

-   filterout: filter title and description

-   filterout_title: filter title only

-   filterout_description: filter description only

-   filterout_author: filter author only

For example: [https://rsshub.app/dribbble/popular?filterout=Blue|Yellow|Black](https://rsshub.app/dribbble/popular?filterout=Blue|Yellow|Black)

### Limit Entries

Set `limit` to limit the number of articles in the feed,

Eg: Dribbble Popular Top 10 [https://rsshub.app/dribbble/popular?limit=10](https://rsshub.app/dribbble/popular?limit=10)

## Fulltext

Enable fulltext via `mode` parameter

Eg: bilibili article <https://rsshub.app/bilibili/user/article/334958638?mode=fulltext>

## Telegram instantview

Replace website link with Telegram instantview link

Eable Telegram instantview needs making page template, refer to [official website](https://instantview.telegram.org/)

-   tgiv: template hash, getting form link of making template page（the string after `&rhash=`）

Eg: <https://rsshub.app/novel/biquge/94_94525?tgiv=bd3c42818a7f7e>

### Output Formats

RSSHub supports RSS 2.0 and Atom as the output formats, simply append `.rss` `.atom` to the end of the feed address, default to RSS 2.0

For example:

-   Default (RSS 2.0) - [https://rsshub.app/dribbble/popular](https://rsshub.app/dribbble/popular)
-   RSS 2.0 - [https://rsshub.app/dribbble/popular.rss](https://rsshub.app/dribbble/popular.rss)
-   Atom - [https://rsshub.app/dribbble/popular.atom](https://rsshub.app/dribbble/popular.atom)
-   Apply filters or URL query [https://rsshub.app/dribbble/popular.atom?filterout=Blue|Yellow|Black](https://rsshub.app/dribbble/popular.atom?filterout=Blue|Yellow|Black)
