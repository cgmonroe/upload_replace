# upload_replace
This is a Drupal 8 version of the D7 upload_replace module.  See https://drupal.org/project/upload_replace for usage details. 

Based on patch supplied by lathan in issue https://www.drupal.org/project/upload_replace/issues/2868450

To use with Composer add the following to the repositories section of your composer.json file:

```
    "cgmonroe.upload_replace": {
      "type" : "package",
      "package" : {
        "name" : "cgmonroe/upload_replace",
        "version" : "8.x-1.x-dev",
        "type" : "drupal-module",
        "dist" : {
          "url" : "https://github.com/cgmonroe/upload_replace/archive/master.zip",
          "type" : "zip"
        },
        "require" : {
          "composer/installers" : "^1.0.21"
        }
      }
    },
```

This assumes that you have the common drupal types set up in the composer file.  E.g.:

```
  "extra" : {
    "installer-paths" : {
      "docroot/core" : [
        "type:drupal-core"
      ],
      "docroot/libraries/{$name}" : [
        "type:drupal-library"
      ],
      "docroot/modules/contrib/{$name}" : [
        "type:drupal-module"
      ],
      "docroot/themes/contrib/{$name}" : [
        "type:drupal-theme"
      ]
    },
  }
```
