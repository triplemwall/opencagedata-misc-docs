  * Full [API docs](https://opencagedata.com/api).
  * We recommend you also [follow us on Mastodon](https://en.osm.town/@opencage) and/or [read our blog](https://blog.opencagedata.com/) where all changes are announced. 

# Changes to OpenCage Geocoder API. 

* 20230801

  As recently announced the `stay_informed` section of our API response has now changed, we no longer provide a reference to Twitter.
  
* 20230724
  
   From 1 August 2023 we will adapt the `stay_informed` portion of our API response to no longer include a reference to our Twitter account. [Details on the blog](https://blog.opencagedata.com/post/dropping-twitter).
  
* 20230323

  We now support searching for UN/LOCODE codes, and, for paying customers, provide UN/LOCODE information as a new annotation. See [the detailed documentation (includign caveats)](https://opencagedata.com/api#unlocode), [blog post](https://blog.opencagedata.com/post/search-for-unlocodes). 

* 20230209

  From 1 March 2023 the price and size of some of our geocoding subscription plans will change for new customers. Existing customers that are impacted by these changes will be contacted by email. [Blog post explaining the details](https://blog.opencagedata.com/post/pricing-changes-coming). 

* 20230113

  We have added a new annotation `NUTS`. See [the annotation documentation](https://opencagedata.com/api#annotations), [blog post](https://blog.opencagedata.com/post/now-with-nuts). 

* 20230110

  * The `stay_informed` portion of our API response now includes a reference to [our Mastodon account](https://en.osm.town/@opencage). 
  * new optional parameter `address_only`. [See documentation](https://opencagedata.com/api#address_only-param).

  [Detailed blog post](https://blog.opencagedata.com/post/new-optional-parameter-addressonly).

* 20221219

  In January 2023 (target date 10 Jan 2023) we will adapt the `stay_informed` portion of our API response to include a reference to our Mastodon account. [Details on the blog](https://blog.opencagedata.com/post/moving-beyond-twitter).

* 20220701

  We have added a new annotation `H3`. See [the annotation documentation](https://opencagedata.com/api#annotations), [blog post](https://blog.opencagedata.com/post/new-annotation-h3).

* 20220516

  If possible we now add a key `ISO_3166-2`to the `components` portion of each result. The value of the field is a list (not a single value) of [ISO 3166-2 codes](https://en.wikipedia.org/wiki/ISO_3166-2) for that location. [Detailed blog post](https://blog.opencagedata.com/post/now-with-iso-3166-2-codes) with many examples, particularly of unexpected edge cases.

* 20220321

  One of the primary geocoders we aggregate behind our API is Nominatim. Yesterday we made the switch to a newer version - Nominatim 4.0 - which introduces significant changes. While we have extensive tests it is difficult to foresee every possible permutation. Please let us know if you are seeing anything unexpected.
  
* 20220215 

  [OpenCage Geosearch](https://opencagedata.com/geosearch) is now available. [Detailed blog post](https://blog.opencagedata.com/post/introducing-opencage-geosearch) 

* 20211016

  Legal headquarters of OpenCage GmbH has now moved to Hannover, Niedersachsen, Germany. [Detailed blog post](https://blog.opencagedata.com/post/we-have-moved).

* 20211001

  [Sign up is now open](https://opencagedata.com/geosearch) for early access to our soon to be launched geosearch service. [Detailed blog post](https://blog.opencagedata.com/post/geosearch-early-access-list-now-open). 

* 20210406

  Reverse geocoding requests that match roads with no names will now set `"road": "unnamed road",` in the `components` sections of results. [Blog post with details](https://blog.opencagedata.com/post/where-the-streets-have-no-name).

* 20200928

  One of the primary geocoders we aggregate behind our API is Nominatim. This morning (European time) we made the switch to a newer version - Nominatim 3.5 - 
  which introduces significant changes to administrative hierarchies in some countries. While we have extensive tests it is difficult to foresee every possible
  permutation. Please let us know if you are seeing anything unexpected in the `formatted` or `components` sections of results. 

* 20200915

  * HTTPS requests with TLS < 1.2 are no longer supported. Invalid requests now return a `426` response. [Blog post with details](https://blog.opencagedata.com/post/deprecation-of-unsecure-tls)
  * `map` output format no longer supported
  
* 20200831

  A reminder that on 15 Sept 2020 we will turn off support for HTTPS API requests using TLS 1.0 or 1.1. We have set up a server for testing for those 
  who have not yet made the transition ([details on our blog](https://blog.opencagedata.com/post/url-for-testing-tls-1point2)). Please make the switch 
  to TLS 1.2+ as quickly as possible to ensure your service continues to work after the 15th of September.
  
* 20200709

  In addition to our existing subscription pricing plans, we now also support [one-time purchases](https://blog.opencagedata.com/post/one-time-purchases).
  
* 20200518

  Deprecation notice: from 15 September 2020

    * all API requests will need to be HTTPS TLS 1.2 or higher
    * we will no longer support the `map` output format

  Please see [our blog post detailing these changes](https://blog.opencagedata.com/post/deprecating-tls-1point0-and-1point1).

* 20200414

  The OpenCage twitter account has changed to [@OpenCage](https://twitter.com/OpenCage). We have accordingly changed the value in the `stay_informed` portion of the API response. 

* 20200413

  We now support requests using the HTTP/2 protocol. [Blog post](https://blog.opencagedata.com/post/supporting-http2).

* 20200403

  Paying customers can now, on a per API key basis, specify a value for the `access-control-allow-origin` HTTP header returned by the API as a way to limit domains on which AJAX requests can be made. [Blog post with details](https://blog.opencagedata.com/post/setting-the-access-control-allow-origin-header).

* 20200325

  Accounts can now be secured with two-factor authentication (2FA). [Blog post](https://blog.opencagedata.com/post/two-factor-authentication).
  
* 20200309

  Paying customers can now specify an allowed list of IP addresses that are able to query the geocoding API with a specific API key. Requests from all other addresses will receive a `403 - IP address rejected` response. [Blog post](https://blog.opencagedata.com/post/ip-restriction).

* 20200120

  We now include a `_category` key and value in the `components`portion of
  each result. [Documentation with link to a list of possible values](https://opencagedata.com/api#formatted). [Blog post](https://blog.opencagedata.com/post/categorization).

* 20191223

  The `OSM` annotation now also contains a `note_url` key and value to make adding a note to OpenStreetMap easier. [Blog post](https://blog.opencagedata.com/post/osm-annotation-notes-url). Learn more [about OpenStreetMap Notes](https://wiki.openstreetmap.org/wiki/Notes). 


* 20191219

  more languages for our `what3words` annotation. The following languages are now supported: ` af,ar,bg,bn,cs,da,de,el,en,es,fi,fr,he,hu,id,it,ja,ko,mn,mr,ms,nl,no,pl,pt,ro,ru,sv,sw,ta,te,th,tr,xh,zh,zu`


* 20191211

  there is now an API key for use in testing and SDK development that will always generate a response with status `200` (as there had previously been for `402`, `403`, and `429`. You can find the key [the section of the API docs dealing with response codes](https://opencagedata.com/api#codes).

* 20191111

  there is now an API key for use in testing and SDK development that will always generate a response with status `429` (as there had previously been for `402` and `403`. You can find the key [the section of the API docs dealing with response codes](https://opencagedata.com/api#codes).

* 20191106

  previously requests with no query (`q` parameter) confusingly returned a `200`response code. Such requests now return `400` response code with the message `missing or bad query`.

* 20191002

  When possible we now also match [terminated postcodes](https://blog.opencagedata.com/post/now-with-old-postcodes). 
  
* 20190715

  the OpenCage geocoding API is now operated by OpenCage GmbH. [Blog post](https://blog.opencagedata.com/post/we-are-now-opencage-gmbh). The value of the `thanks` field of the API response has changed slightly, as explained in the blog post.

* 20190709

  due to some architectural refactoring to handle increased usage, we have turned off the `OSGB` annotation. We hope to have it back soon. 

* 20190708

  if `language=native` has been specified we will attempt to return results in the local "official" language. See [blog post](https://blog.opencagedata.com/post/support-for-local-language) for details, links to documentation and caveats.

* 20190517

  we have added a new annotation `UN_M49`. See [the annotation documentation](https://opencagedata.com/api#annotations), [blog post](https://blog.opencagedata.com/post/new-annotation-un-m49-statistical-codes)

* 20190430
 
  new optional parameter `roadinfo`, which tells the API to attempt to match 
  roads and add information like speed limits. 
  See [documentation](https://opencagedata.com/api#roadinfo), [blog post](https://blog.opencagedata.com/post/new-optional-parameter-roadinfo)

* 20190426

  we have added a new annotation `roadinfo`. See [the annotation documentation](https://opencagedata.com/api#annotations). 

* 20190425

  We've changed the content of the `licenses` portion of our response format
  to point to [our attribution page](https://opencagedata.com/credits).
  See [response format documentation](https://opencagedata.com/api#response)
  
* 20190423

  To aid in debugging we now return HTTP response code `401` in the case when either no API key is supplied in the request, or an invalid API key is supplied. Previously we had returned a `403` response in this situation.
  See details of all [the various response codes the API can return](https://opencagedata.com/api#codes).

* 20190219

  when possible we now also return a `continent` key and value in the `components` portion of each result. [See blog post](https://blog.opencagedata.com/post/now-with-continents).
   
* 20190102

  map view upgraded to leaflet 1.4.0 

* 20190101

  we now have a couple of publicly available API keys for use in testing and SDK development that will always generate a response with status `402` and `403`, respectively. You can find them in [the section of the API docs dealing with response codes](https://opencagedata.com/api#codes).
  
* 20181219

  we now also return a `ISO_3166-1_alpha-3` key and value in the `components` portion of each result. [See blog post](https://blog.opencagedata.com/post/now-with-iso3166-1-alpha-3-codes).
  
* 20180923
  
  new version of the what3words library for our annotation means that we now support Afrikaans, Czech, Danish, Dutch, Greek, Japanese, Korean, Norwegian, Thai, Xhosa, and Zulu.

* 20180902
  
  we have significantly improved the granularity and coverage of [our timezone annotation](https://opencagedata.com/api#annotations).

* 20180827
  
  previously results in `geojson` format had not returned some of the fields (examples include `status`, `timestamp`, and more) that other response formats had. This is now corrected, sorry for the oversight.

* 20180801
  
  non-GET HTTP requests to the API now return `405 - Method not allowed` error.
  
* 20180727

   added `FIPS` annotation for locations in the United States. [See docs](https://opencagedata.com/api#annotations).
  
* 20180724

  New optional parameter `proximity` for biasing results is now supported. [See docs](https://opencagedata.com/api#forward-opt).
  
* 20180701

  From 1 August 2018 non-GET HTTP requests will be treated as errors. Please see [our blog post for full details](https://blog.opencagedata.com/post/no-longer-supporting-non-get-requests).

* 20180619

  our website moved to [https://opencagedata.com](https://opencagedata.com).

* 20180618

  added [the Australian G-NAF dataset](https://data.gov.au/dataset/geocoded-national-address-file-g-naf) as one of the backend geocoders we query.

* 20180614
  
  if a result is a road (ie `_type` key in the `components` portion of the result has the value "road") if possible we now also return a `road_type` with values like those [generally used in OpenStreetMap](https://wiki.openstreetmap.org/wiki/Key:highway).

* 20180403
  
  added [the Addok geocoder](http://addok.readthedocs.io/fr/latest/) as one of the backend geocoders we query.
  
* 20180302

  new page to clarify [GDPR/data protection](https://opencagedata.com/gdpr)

* 20171203

   added `flag` annotation. See [the full list of annotations](https://opencagedata.com/api#annotations).

* 20171005
  
   In many parts of the world roads may have names but also numbers or some sort of unique identifier code. In cases where the result for a reverse geocoding query is such a road, the `components` portion of the response now also contains a `road_reference` key and value. In Europe some major highways may also have a national and European reference (for example "A 6" and "E 15"). In such cases we also set the `road_reference_intl` key and value.

* 20170601
  
   the `components` portion of the result now contains the key `ISO_3166-1_alpha-2` with [the corresponding code](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) for that location if we are able to determine it. This is in addition to the two-letter `country_code` which is also returned. This is mainly useful for places like Puerto Rico or Guadeloupe where the two codes differ. 
   
* 20170517

    We have launched a new account dashboard, removing the 3rd party dashboard from 3scale we had peviously used. Passwords in the old (and new) systems were encrypted, thus making it impossible for us to transfer them to the new system, so the first time you log into the new system you will have to create a new password. Sorry for the inconvenience. 

* 20170428

    new optional parameter `abbrv`. When supplied we attempt to shorten the `formatted` string that we return. 
    Abbreviations are open-sourced [in the address-formatting repo](https://github.com/OpenCageData/address-formatting/tree/master/conf/abbreviations).
    See [all optional parameters](https://opencagedata.com/api#forward-opt).
    

* 20170415

    new version of the what3words library for our annotation means that we now support Arabic, Finnish, Italian, Mongolian, Polish, and Swedish
    
* 20170311

    some tweaks to how we calculate [confidence score](https://opencagedata.com/api#confidence) for some of the backend geocoders, will generally result in slightly lower confidence
    
* 20170111

   requests to geocode invalid coordinates now return a response with status code 400 [Blog post](http://blog.opencagedata.com/post/155733527528/change-to-coordinate-handling).

* 20161219

   added `wikidata` annotation. 
 
* 20161028

   added `qibla` annotation. [Blog post](http://blog.opencagedata.com/post/152418938118/new-annotation-qibla).
   
* 20161020

   added `currency` annotation.
   [Blog post](http://blog.opencagedata.com/post/152063767603/new-annotation-currency).

* 20161007

   map view upgraded to leaflet 1.0.1 
   
* 20160914

   The optional parameter `countrycode` can be a comma seperated list of 2-letter country codes  [See full list of optional parameters](https://opencagedata.com/api#forward-opt).

* 20160830

   Previously if a road name in the components field had been a digit it had been returned as a number not a string. This was unintentional and is now fixed. The road name is always returned as a string.

* 20160601

   new optional request parameter `no_record`. [See full list of optional parameters](https://opencagedata.com/api#forward-opt).

* 20160503
   
   tweak to `google-v3-json` format to convert our types to google types
   
* 20160423
   
   add `_type` key to the `components` list so that the type of object we geocoded to can more easily be determined. [See docs](https://opencagedata.com/api#formatted).
   
