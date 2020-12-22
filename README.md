# Wordpress fork

Detta är en fork av [Wordpress](https://github.com/WordPress/WordPress).

Tanken är att denna fork ska användas som bas för wordpress-siter, 
och att siterna därmed kan uppgraderas när nya versioner av 
wordpress släpts via git utan ytterligare modifieringar.

Följande ändringar har gjorts gentemot original-repot:

* .gitignore är tillagd
* wp-content mappen är borttagen
* Readmefilen är tillagd

## Installation

1. Klona detta repo
2. Välj en tagg (version) att jobba mot:
	* `git fetch --tags`: Uppdatera taggar
	* `git tag -l`: Lista tillgängliga taggar
	* `git checkout [tag]`: Checka ut en tagg
	* Taggar markerade med `-baked` är preparerade och klara att användas. 
	  Om den tagg du vill använda inte har en `-baked`-version eller om
	  taggen saknas helt bör du baka den tagg du vill använda, se
	  nedan för instruktioner.
3. Skapa en wp-config.php with
    * WP_CONTENT_DIR
    * WP_CONTENT_URL
    * WP_SITEURL
    * WP_HOME

## Uppgradering

För att uppgradera Wordpress på en site kör du en pull på detta repo, 
därefter loggar du in i wp-admin.
