# Currency Convertor

DEV Blueprint Link!  Remove before push to main!!

[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fraw.githubusercontent.com%2Fdinki%2FView-Assist%2Fviewassist-currencyconvertor%2FView+Assist+custom+sentences%2FCurrency+Convertor%2Fblueprint-currencyconvertor.yaml)

Prequisites:
* You must have Pyscript installed [See installation video](https://www.youtube.com/watch?v=jpJxZaisbGQ)
* You must get an API key from rapidapi.com for the [required API](https://rapidapi.com/pwshub-pwshub-default/api/crypto-market-prices) (totally free no credit card needed)
* You must add your API key to the 'rapidapikey' field in the blueprint
* Download
  * 'viewassist-currencyconvertor.py'
  * 'viewassist-response_handler.py'
  * 'viewassist_currencyconvertor_digits.yaml'
  and place this files in your 'pyscripts' directory on your Home Assistant server
* The pyscript variables **hass_all_imports** and **hass_is_global** need to be set to true. This can be done in the UI or via an entry
> pyscript:
>   allow_all_imports: true
>   hass_is_global: true
in configuration.yaml
* If not exist create a directory 'intent_script' in your 'config' directory on your Home Assistant server.
* Download 'viewassist_currenyconvertor.intent.yaml' and place it in this 'inten_script' directory.
* The **intent_script** directory must be accessed via the entry
> intent_script: !include_dir_merge_named intent_script/
in **configuration.yaml**.
* If not exist create a directory 'custom_sentences' in your 'config' directory on your Home Assistant server.
* if not exist create your preferred language directory (esp. 'en') in this 'custom_sentences' directory.
* Download the
  * 'viewassist_currencyconvertor_intent.yaml'
  * 'viewassist_currencyconvertor_response.yaml'
  * 'viewassist_currencyconvertor_currencies.yaml'
  files from your preferred language directory (esp. 'en') and place this files in the corresponding language directory on your Home Assistant server.
