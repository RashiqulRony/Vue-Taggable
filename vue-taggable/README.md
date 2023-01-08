# Vue Taggable

<p align="center">
<img style="width: 100%" src="https://raw.githubusercontent.com/RashiqulRony/rony.mmj/master/ezgif.com-gif-maker.gif" alt="download" border="0" />
</p>

## Installation

## Usage

```html
<InputTag v-model="tags"/>
```

## Props
| Name | Type | Default | Description |
| ---:| --- | ---| --- |
| value | Array | [] | Tags to be render in the input |
| placeholder | String | "" | Placeholder to be shown when no tags |
| read-only | Boolean | false | Set input to readonly |
| add-tag-on-blur | Boolean | false | Add tag on input blur |
| limit | String or Number | -1 (none) | Set a limit for the amount of tags |
| validate | String or Function (allows async) or Object | "" | Apply certain validator for user input. Choose from `email`, `url`, `text`, `digits` or `isodate`. Or pass a `function` or a `RegExp` object for custom validation |
| add-tag-on-keys | Array | [ 13 (return), 188 (comma), 9 (tab) ] | Keys that are going to add the new tag
| allow-duplicates | Boolean | false | Allow duplicate tags
| before-adding | Function | null | Function (allows async) to normalize tag before adding. E.g `(tag) => tag.toUpperCase()`

## Events
| Name | Arguments | Description |
| ---: | --- | --- |
| input | Array with tags | Emitted when a tag is added (after successful validation) and when a tag is removed |
| update:tags | Array with tags | Same as input event |
