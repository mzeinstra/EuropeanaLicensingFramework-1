#Available Rights Statements

Europeana's [Data Exchange Agreement](http://pro.europeana.eu/data-exchange-agreement) requires that data providers apply a rights statement for all digital objects described in their metadata. The rights that apply to the digital object will also apply to the previews used in the Europeana portal. This rights statement is stored in the 'europeana:rights' field of the [Europeana Semantic Elements](http://www.europeana.eu/schemas/ese/) (ESE) and in the 'edm:rights' field of the [Europeana Data Model](http://www.europeana.eu/schemas/edm/) (EDM). This page gives more information on how to provide such a rights statement.

##General

Only one rights statement can be provided per resource. Rights statements are encoded as URLs referring to webpages that contain information about the applicable rights. The webpages inform the user about the terms under which the digital object and the corresponding preview can be used. Most of the examples on this page use the ESE standard but are also applicable when using EDM:

> <europeana:rights>http://a.rights.statement/</europeana:rights>

 or

> <edm:rights>http://a.rights.statement/</edm:rights>

Alongside each preview, Europeana will display a rights statement icon. This is based on the value in 'europeana:rights' or 'edm:rights'. Clicking the icon will take the user to a webpage explaining the statement.

Europeana allows its users to filter search results based on rights statements. This means searches can be restricted so that users only find objects that they are allowed to re-use. This functionality is also available via the Europeana API, allowing developers to work with subsets of information based on rights status.

##Types of Rights Statements

There are four different types of rights statement. These are listed here and explained more fully below:

* Objects that are not protected by copyright and can therefore be freely re-used must be marked as being in the public domain by applying the Public Domain Mark (see 1 below).
* When the data provider is also the rights holder and wants to make the digital object available for re-use (or has been authorised by the rights holder to do so) the data provider can apply a Creative Commons Licence or the CC0 1.0 Universal Public Domain Dedication (see 2 - 8 below).
* When the data provider is also the rights holder and wants to make the digital object available without authorising re-use by third parties (or has been authorised by the rights holder to do so), the data provider can apply one of the three standardised Rights Reserved statements developed by Europeana (see 9 - 11 below).
* Objects with a copyright status that is unclear (for example because no rights holder could be identified) can be marked with an 'unknown' copyright statement. This should only be used if absolutely necessary (see 12 below). 

Within these four types, there are 12 separate statements that can be applied to a particular object.

##Available Rights Statements

###<a name="Public_Domain_Mark">1 The Public Domain Mark (PDM)</a>

All content that is in the public domain must be labelled accordingly. Europeana has worked with Creative Commons to develop a simple mark that indicates that a work is in the public domain - the Public Domain Mark. Works that are labelled as being in the public domain can be used by anyone without any restrictions. When showing the Public Domain Mark, Europeana will also link to [Europeana Usage Guidelines for public domain works](http://www.europeana.eu/portal/rights/pd-usage-guide.html).

The URL to use in the metadata is: [http://creativecommons.org/publicdomain/mark/1.0/](http://creativecommons.org/publicdomain/mark/1.0/)

> <europeana:rights>http://creativecommons.org/publicdomain/mark/1.0/</europeana:rights>

[Examples of objects with this rights statement on Europeana](http://www.europeana.eu/portal/search.html?query=RIGHTS%3A*mark*).

###<a name="CC0">2 The Creative Commons CC0 1.0 Universal Public Domain Dedication (CC0)</a>

If a rights holder wants to waive all the rights in a digital object, they can apply a CC0 waiver to the works in question. By applying this waiver, all rights in the content are waived and the objects can be used by anyone without any restrictions. CC0 can only be applied with the authority of the rights holder.

The URL to use in the metadata is: [http://creativecommons.org/publicdomain/zero/1.0/](http://creativecommons.org/publicdomain/zero/1.0/)

> <europeana:rights>http://creativecommons.org/publicdomain/zero/1.0/</europeana:rights>

[Examples of objects with this rights statement on Europeana](http://www.europeana.eu/portal/search.html?query=RIGHTS%3A*zero*).

###<a name="CC">Creative Commons Licences</a>

The Creative Commons (CC) licences provide options for copyright holders to allow others to re-use digitised objects under certain conditions. The CC licences can only be applied with permission from the rights holder.

The following six CC licenses can be used as rights statements for digital objects in Europeana. The licences are summarised below using the words from the CC website and are presented in order from the most open to the most restrictive. It is strongly recommended that you refer to the [Creative Commons website](http://creativecommons.org/licenses/ ) to see the full definitions and legal code when making your decision.

The CC licences also exist as jurisdiction-specific licences. Europeana supports all available jurisdiction versions, however, the examples given below use the URLs of the 'universal' licences. If you want to make objects available under a jurisdiction-specific Creative Commons licence, you are advised to use the [selection tool](http://www.creativecommons.org/choose/) on the Creative Commons website. This will give you the correct licence URL for the 'edm:rights' field.

###<a name="CC-BY">3 Creative Commons - Attribution (BY)</a>

This licence lets others distribute, remix, tweak, and build upon your work, even commercially, as long as they credit you for the original creation. This is the most accommodating of licences offered. Recommended for maximum dissemination and use of licensed materials.

The URL to use in the metadata is: [http://creativecommons.org/licenses/by/3.0/](http://creativecommons.org/licenses/by/3.0/)

> <europeana:rights>http://creativecommons.org/licenses/by/3.0/<europeana:rights>

[Examples of objects with this rights statement on Europeana](http://www.europeana.eu/portal/search.html?query=*:*&amp;qf=RIGHTS:http://creativecommons.org/licenses/by/*).

###<a name="CC-BY-SA">4 Creative Commons - Attribution, ShareAlike (BY-SA)</a>

This licence lets others remix, tweak, and build upon your work even for commercial purposes, as long as they credit you and licence their new creations under the identical terms. This licence is often compared to 'copyleft', free and open source software licences. All new works based on yours will carry the same licence, so any derivatives will also allow commercial use. This is the licence used by Wikipedia, and is recommended for materials that would benefit from incorporating content from Wikipedia and similarly licensed projects.

The URL to use in the metadata is: [http://creativecommons.org/licenses/by-sa/3.0/](http://creativecommons.org/licenses/by-sa/3.0/)

> <europeana:rights>http://creativecommons.org/licenses/by-sa/3.0/<europeana:rights>

[Examples of objects with this rights statement on Europeana](http://www.europeana.eu/portal/search.html?query=RIGHTS%3A*by-sa*).

###<a name="CC-BY-ND">5 Creative Commons - Attribution, No Derivatives (BY-ND)</a>

This licence allows for redistribution, commercial and non-commercial, as long as it is passed along unchanged and in whole, with credit to you.

The URL to use in the metadata is: [http://creativecommons.org/licenses/by-nd/3.0/](http://creativecommons.org/licenses/by-nd/3.0/)

> <europeana:rights>http://creativecommons.org/licenses/by-nd/3.0/<europeana:rights>

[Examples of objects with this rights statement on Europeana](http://www.europeana.eu/portal/search.html?query=RIGHTS%3A*by-nd*).

###<a name="CC-BY-NC">6 Creative Commons - Attribution, Non-Commercial (BY-NC)</a>

This licence lets others remix, tweak, and build upon your work non-commercially, and although their new works must also acknowledge you and be non-commercial, they don't have to licence their derivative works on the same terms.

The URL to use in the metadata is: [http://creativecommons.org/licenses/by-nc/3.0/](http://creativecommons.org/licenses/by-nc/3.0/)

> <europeana:rights>http://creativecommons.org/licenses/by-nc/3.0/<europeana:rights>

[Examples of objects with this rights statement on Europeana](http://www.europeana.eu/portal/search.html?query=*:*&amp;qf=RIGHTS:http://creativecommons.org/licenses/by-nc/*).

###<a name="CC-BY-NC-SA">7 Creative Commons - Attribution, Non-Commercial, ShareAlike (BY-NC-SA)</a>

This licence lets others remix, tweak, and build upon your work non-commercially, as long as they credit you and licence their new creations under the identical terms.

The URL to use in the metadata is: [http://creativecommons.org/licenses/by-nc-sa/3.0/](http://creativecommons.org/licenses/by-nc-sa/3.0/)

> <europeana:rights>http://creativecommons.org/licenses/by-nc-sa/3.0/<europeana:rights>

[Examples of objects with this rights statement on Europeana](http://www.europeana.eu/portal/search.html?query=RIGHTS%3A*by-nc-sa*).

###<a name="CC-BY-NC-ND">8 Creative Commons - Attribution, Non-Commercial, No Derivatives (BY-NC-ND)</a>

This licence is the most restrictive of our six main licences, only allowing others to download your works and share them with others as long as they credit you, but they can't change them in any way or use them commercially.

The URL to use in the metadata is: [http://creativecommons.org/licenses/by-nc-nd/3.0/](http://creativecommons.org/licenses/by-nc-nd/3.0/)

> <europeana:rights>http://creativecommons.org/licenses/by-nc-nd/3.0/<europeana:rights>

[Examples of objects with this rights statement on Europeana](http://www.europeana.eu/portal/search.html?query=RIGHTS%3A*by-nc-nd*).

###Europeana Rights Reserved Statements

For data providers who do not want to or cannot allow object re-use, Europeana has developed three standard rights statements. These statements express the conditions under which objects can be accessed on the data provider's website. Use of these statements means the data provider is reserving the rights in the digital object and that the object may not be used without additional permissions.

###<a name="RR-F">9 Rights Reserved - Free Access</a>

This rights statement is applicable when users have free (as in gratis), direct and full access to the digitised object on the data provider's website.

The URL to use in the metadata is: [http://www.europeana.eu/rights/rr-f/](http://www.europeana.eu/rights/rr-f/)

> <europeana:rights>http://www.europeana.eu/rights/rr-f/</europeana:rights>

[Examples of objects with this rights statement on Europeana](http://www.europeana.eu/portal/search.html?query=RIGHTS%3A*rr-f*).

###<a name="RR-P">10 Rights Reserved - Paid Access</a>

This rights statement is applicable when users need to pay data providers to gain access to the digitised work on the data provider's website. This may be the case if only a preview is accessible through the data provider's portal, and registration and payment is required to gain access to the digitised object itself. In this case, the link from Europeana should give access to the metadata and (ideally) a low-resolution preview. Europeana will not link directly to a payment page.

The URL to use in the metadata is: [http://www.europeana.eu/rights/rr-p/](http://www.europeana.eu/rights/rr-p/)

> <europeana:rights>http://www.europeana.eu/rights/rr-p/</europeana:rights>

[Examples of objects with this rights statement on Europeana](http://www.europeana.eu/portal/search.html?query=RIGHTS%3A*rr-p*).

###<a name="RR-R">11 Rights Reserved - Restricted Access</a>

This rights statement is applicable when there are limitations other than the requirement to pay a fee for accessing a digitised object on the data provider's website. For example, when a registration is required or only snippets or previews are available to users. In this case, the link from Europeana should give access to the metadata and (ideally) a low-resolution preview. Europeana will not link directly to a registration page.

The URL to use in the metadata is: [http://www.europeana.eu/rights/rr-r/](http://www.europeana.eu/rights/rr-r/)

> <europeana:rights>http://www.europeana.eu/rights/rr-r/</europeana:rights>

[Examples of objects with this rights statement on Europeana](http://www.europeana.eu/portal/search.html?query=RIGHTS%3A*rr-r*).

###<a name="unknown">12 Unknown</a>

The Unknown rights statement can be applied to objects for which the data provider does not have conclusive information pertaining to the rights status of the digital object (e.g. orphan works). This value is only to be used when the copyright status of the work described is unknown. This statement may be used by Europeana to exclude items from display and should therefore not be used without consultation with the Europeana Ingestion team.

The URL to use in the metadata is: [http://www.europeana.eu/rights/unknown/](http://www.europeana.eu/rights/unknown/)

> <europeana:rights>http://www.europeana.eu/rights/unknown/</europeana:rights>

[Examples of objects with this rights statement on Europeana](http://www.europeana.eu/portal/search.html?query=RIGHTS%3A*unknown*).

##What is the difference between the Creative Commons Licences and the Europeana Rights Reserved statements?

Creative Commons licences allow re-use of the licensed object, while the Europeana Rights Reserved statements simply indicate under which conditions the object may be accessed (but not re-used).

**Creative Commons licences:**

* Allow re-use of the digital objects under certain conditions
* May therefore only be applied by the rights holder or with permission from the rights holder 

**Europeana Rights Reserved Statements:**

* Indicate that users can access the digital objects but that they are not allowed to re-use them
* Should be applied by the rights holder or after the rights in the digital object have been created by the data provider 

##What is the difference between the Public Domain Mark and the CC0 Public Domain Dedication?

 It is very important not to confuse these two rights statements. It will often be the case that cultural heritage digital objects submitted to Europeana will be in the public domain and must be marked accordingly by using the Public Domain Mark. CC0 is specifically designed for use with (meta) data sets and is unlikely to be used as a rights statement describing content. In the context of Europeana, CC0 is primarily used to ensure that metadata can be used without any restrictions. The CC0 waiver is automatically applied to all metadata that is being provided to Europeana.

**The Public Domain Mark (PDM):**

* Applies to objects that are not subject to copyright either because copyright has expired (e.g. the author died many years ago) or because the object was never subject to such rights and is therefore in the public domain.
* Anyone can apply the PDM to an object if they know the object is in the public domain. 

**The Creative Commons CC0 1.0 Universal Public Domain Dedication:**

* Can be applied to objects or data that is subject to copyright but where the rights holder wants to waive the rights and dedicate the object to the public domain.
* It can only be applied by the rights holder or someone who is authorised by the rights holder.