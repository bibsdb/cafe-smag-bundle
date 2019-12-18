# bibsdb/cafe-smag

Supplies a slide template for playing cafe-smag videos. This bundle uses CafeSmag's js player: https://github.com/cafe-smag/player.js/

## Installation

Add the git repository to "repositories" in `composer.json`.

<pre>
"repositories": {
    "bibsdb/cafe-smag-bundle": {
      "type": "vcs",
      "url": "https://github.com/bibsdb/cafe-smag-bundle"
    },
    ...
}
</pre>

Require the bundle with composer.

<pre>
composer require bibsdb/cafe-smag-bundle
</pre>

Enable the bundle in `AppKernel.php`, by adding BibsdbCafeSmagBundle to $bundles.

<pre>
new Bibsdb\CafeSmagBundle\BibsdbCafeSmagBundle()
</pre>

Run bibsdb:core:templates:load command to load the template in the installation.

<pre>
bin/console bibsdb:core:templates:load
</pre>

Enable the template in the administration.

## Ads and controls

To avoid ads and video controls, the shared video has to come from a user
that has disabled the options at cafe-smag.com. To do it yourself, you need to have
at least a PLUS account (https://cafe-smag.com/plus).
