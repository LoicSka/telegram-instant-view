### How to achieve instant view on telegram

Currently there are 4 ways to get Instant View for your website:

- Mimic a Medium page (fastest + easiest)
- Mimic a WordPress/Telegraph/Zen etc. (hardest)
- Create and use your own Instant View Template
- Suggest Telegram to make IV for your site (press “Add Domain”)

#### Here is how you can achieve the first option.

### Meta tags

The following two tags will trick Telegram into using Medium template for our site.

``` html
<meta property="al:android:app_name" content="Medium" />
```
This will make Telegram use Medium template for our article. As far as we know this does not break anything, even if user has Android Medium app installed.
```html
<meta property="article:published_time" content="2020-02-02T00:00:00.000Z" />
```

Additional tags are used to set up webpage preview (the block you see in the chat above Instant View button). These are optional.

```html
<meta property="og:site_name" content="SITE_NAME" />
```

Shows correct site name instead of default “Medium”.

```html
<meta property="og:description" content="DESCRIPTION"  />
```

A short description.

```html
<meta property="og:image" content="PREVIEW_IMAGE_URL" />
```
A preview image.

Following tags modify parts of the Instant View page itself.

```html
<meta name="author" content="AUTHOR_NAME" />
```

Author name will be shown below title next to the date. Add multiple tags for multiple authors.

```html
<meta name="telegram:channel" content="@YOUR_CHANNEL" />
```

A link to a Telegram channel with a “Join” button can be shown at the top of the article. Note that this value must start with


For more details about this, check out [this article](http://bit.ly/2AWWzkD)




