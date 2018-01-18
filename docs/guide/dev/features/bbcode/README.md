---
category: output-control
order: 80
url: guide/dev_bbcode
menu-title: BBCode Editing
meta-title-short: BBCode Editing
---
<!--
Copyright (c) 2003-2017, CKSource - Frederico Knabben. All rights reserved.
For licensing, see LICENSE.md.
-->

# BBCode Editing

<info-box info="">
</info-box>

[BBCode](http://en.wikipedia.org/wiki/BBCode) is a lightweight markup language which is used in some message board engines. An optional CKEditor plugin called [BBCode Output Format](https://ckeditor.com/cke4/addon/bbcode) configures CKEditor to output BBCode format instead of (X)HTML. It also customizes some editor settings to better match the BBCode environment.

The image below shows an example of the editor content created in BBCode format, as displayed in the {@link guide/dev/features/sourcearea/README source view}.

{@img assets/img/bbcode_02.png}

## Customizing CKEditor to Work on BBCode

This feature is aimed at developers who would like to integrate CKEditor with popular message boards or other platforms that use BBCode as their default format. Since BBCode formatting usually includes a subset of features available in traditional HTML editing, CKEditor used in this environment needs some customization. This involves creating a [custom editor build](https://ckeditor.com/cke4/builder) that only includes relevant features, {@linkapi CKEDITOR.config#removeButtons removing redundant buttons} or customizing some plugin options (like adjusting smilies).

<info-box hint="">
</info-box>

## BBCode Output Demo

See the [working "BBCode Editing" sample](https://sdk.ckeditor.com/samples/bbcode.html) that showcases a CKEditor instance configured to output BBCode and customized to be a better fit for a typical BBCode environment.

## Related Features

See the {@link guide/dev/features/sourcearea/README Source Code Editing} feature that lets the users edit raw BBCode source of the editor content directly in CKEditor.