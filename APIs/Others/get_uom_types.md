# Retrieve a list of countries with query builder

### URL

```text
api/v1/countries
```

### Method

```text
GET
```

### Parameters

| Name  | Type   | Required | Default | Description |
|-------|--------|----------|---------|-------------|
| iso_2 | string |          |         |             |
| iso_3 | string |          |         |             |

### Note

```text
* `maximum of limit < 200 per page.`
* `paginated data will give out if no flag of list.`

```

### Auth required

```text
Yes
```

### Headers

```text
Content-Type: application/json
Accept: application/json
Authorization: Bearer ******************

```
|country_id|iso2|name                                      |
|----------|----|------------------------------------------|
|1         |AF  |Afghanistan                               |
|2         |AL  |Albania                                   |
|3         |DZ  |Algeria                                   |
|4         |AS  |American Samoa                            |
|5         |AD  |Andorra                                   |
|6         |AO  |Angola                                    |
|7         |AI  |Anguilla                                  |
|8         |AQ  |Antarctica                                |
|9         |AG  |Antigua and Barbuda                       |
|10        |AR  |Argentina                                 |
|11        |AM  |Armenia                                   |
|12        |AW  |Aruba                                     |
|13        |AU  |Australia                                 |
|14        |AT  |Austria                                   |
|15        |AZ  |AzerbaijanEn                              |
|16        |BS  |Bahamas                                   |
|17        |BH  |Bahrain                                   |
|18        |BD  |Bangladesh                                |
|19        |BB  |Barbados                                  |
|20        |BY  |Belarus                                   |
|21        |BE  |Belgium                                   |
|22        |BZ  |Belize                                    |
|23        |BJ  |Benin                                     |
|24        |BM  |Bermuda                                   |
|25        |BT  |Bhutan                                    |
|26        |BO  |Bolivia                                   |
|27        |BA  |Bosnia and Herzegovina                    |
|28        |BW  |Botswana                                  |
|29        |BV  |Bouvet Island                             |
|30        |BR  |Brazil                                    |
|31        |IO  |British Indian Ocean Territory            |
|32        |BN  |Brunei Darussalam                         |
|33        |BG  |Bulgaria                                  |
|34        |BF  |Burkina Faso                              |
|35        |BI  |Burundi                                   |
|36        |KH  |Cambodia                                  |
|37        |CM  |Cameroon                                  |
|38        |CA  |Canada                                    |
|39        |CV  |Cape Verde                                |
|40        |KY  |Cayman Islands                            |
|41        |CF  |Central African Republic                  |
|42        |TD  |Chad                                      |
|43        |CL  |Chile                                     |
|44        |CN  |China                                     |
|45        |CX  |Christmas Island                          |
|46        |CC  |Cocos (Keeling) Islands                   |
|47        |CO  |Colombia                                  |
|48        |KM  |Comoros                                   |
|49        |CG  |Congo                                     |
|50        |CK  |Cook Islands                              |
|51        |CR  |Costa Rica                                |
|52        |CI  |Cote D'Ivoire                             |
|53        |HR  |Croatia                                   |
|54        |CU  |Cuba                                      |
|55        |CY  |Cyprus                                    |
|56        |CZ  |Czech Republic                            |
|57        |DK  |Denmark                                   |
|58        |DJ  |Djibouti                                  |
|59        |DM  |Dominica                                  |
|60        |DO  |Dominican Republic                        |
|61        |TL  |East Timor                                |
|62        |EC  |Ecuador                                   |
|63        |EG  |Egypt                                     |
|64        |SV  |El Salvador                               |
|65        |GQ  |Equatorial Guinea                         |
|66        |ER  |Eritrea                                   |
|67        |EE  |Estonia                                   |
|68        |ET  |Ethiopia                                  |
|69        |FK  |Falkland Islands (Malvinas)               |
|70        |FO  |Faroe Islands                             |
|71        |FJ  |Fiji                                      |
|72        |FI  |Finland                                   |
|74        |FR  |France, Metropolitan                      |
|75        |GF  |French Guiana                             |
|76        |PF  |French Polynesia                          |
|77        |TF  |French Southern Territories               |
|78        |GA  |Gabon                                     |
|79        |GM  |Gambia                                    |
|80        |GE  |Georgia                                   |
|81        |DE  |Germany                                   |
|82        |GH  |Ghana                                     |
|83        |GI  |Gibraltar                                 |
|84        |GR  |Greece                                    |
|85        |GL  |Greenland                                 |
|86        |GD  |Grenada                                   |
|87        |GP  |Guadeloupe                                |
|88        |GU  |Guam                                      |
|89        |GT  |Guatemala                                 |
|90        |GN  |Guinea                                    |
|91        |GW  |Guinea-Bissau                             |
|92        |GY  |Guyana                                    |
|93        |HT  |Haiti                                     |
|94        |HM  |Heard and Mc Donald Islands               |
|95        |HN  |Honduras                                  |
|96        |HK  |Hong Kong                                 |
|97        |HU  |Hungary                                   |
|98        |IS  |Iceland                                   |
|99        |IN  |India                                     |
|100       |ID  |Indonesia                                 |
|101       |IR  |Iran (Islamic Republic of)                |
|102       |IQ  |Iraq                                      |
|103       |IE  |Ireland                                   |
|104       |IL  |Israel                                    |
|105       |IT  |Italy                                     |
|106       |JM  |Jamaica                                   |
|107       |JP  |Japan                                     |
|108       |JO  |Jordan                                    |
|109       |KZ  |Kazakhstan                                |
|110       |KE  |Kenya                                     |
|111       |KI  |Kiribati                                  |
|112       |KP  |North Korea                               |
|113       |KR  |South Korea                               |
|114       |KW  |Kuwait                                    |
|115       |KG  |Kyrgyzstan                                |
|116       |LA  |Lao People's Democratic Republic          |
|117       |LV  |Latvia                                    |
|118       |LB  |Lebanon                                   |
|119       |LS  |Lesotho                                   |
|120       |LR  |Liberia                                   |
|121       |LY  |Libyan Arab Jamahiriya                    |
|122       |LI  |Liechtenstein                             |
|123       |LT  |Lithuania                                 |
|124       |LU  |Luxembourg                                |
|125       |MO  |Macau                                     |
|126       |MK  |FYROM                                     |
|127       |MG  |Madagascar                                |
|128       |MW  |Malawi                                    |
|129       |MY  |Malaysia                                  |
|130       |MV  |Maldives                                  |
|131       |ML  |Mali                                      |
|132       |MT  |Malta                                     |
|133       |MH  |Marshall Islands                          |
|134       |MQ  |Martinique                                |
|135       |MR  |Mauritania                                |
|136       |MU  |Mauritius                                 |
|137       |YT  |Mayotte                                   |
|138       |MX  |Mexico                                    |
|139       |FM  |Micronesia, Federated States of           |
|140       |MD  |Moldova, Republic of                      |
|141       |MC  |Monaco                                    |
|142       |MN  |Mongolia                                  |
|143       |MS  |Montserrat                                |
|144       |MA  |Morocco                                   |
|145       |MZ  |Mozambique                                |
|146       |MM  |Myanmar                                   |
|147       |NA  |Namibia                                   |
|148       |NR  |Nauru                                     |
|149       |NP  |Nepal                                     |
|150       |NL  |Netherlands                               |
|151       |AN  |Netherlands Antilles                      |
|152       |NC  |New Caledonia                             |
|153       |NZ  |New Zealand                               |
|154       |NI  |Nicaragua                                 |
|155       |NE  |Niger                                     |
|156       |NG  |Nigeria                                   |
|157       |NU  |Niue                                      |
|158       |NF  |Norfolk Island                            |
|159       |MP  |Northern Mariana Islands                  |
|160       |NO  |Norway                                    |
|161       |OM  |Oman                                      |
|162       |PK  |Pakistan                                  |
|163       |PW  |Palau                                     |
|164       |PA  |Panama                                    |
|165       |PG  |Papua New Guinea                          |
|166       |PY  |Paraguay                                  |
|167       |PE  |Peru                                      |
|168       |PH  |Philippines                               |
|169       |PN  |Pitcairn                                  |
|170       |PL  |Poland                                    |
|171       |PT  |Portugal                                  |
|172       |PR  |Puerto Rico                               |
|173       |QA  |Qatar                                     |
|174       |RE  |Reunion                                   |
|175       |RO  |Romania                                   |
|176       |RU  |Russian Federation                        |
|177       |RW  |Rwanda                                    |
|178       |KN  |Saint Kitts and Nevis                     |
|179       |LC  |Saint Lucia                               |
|180       |VC  |Saint Vincent and the Grenadines          |
|181       |WS  |Samoa                                     |
|182       |SM  |San Marino                                |
|183       |ST  |Sao Tome and Principe                     |
|184       |SA  |Saudi Arabia                              |
|185       |SN  |Senegal                                   |
|186       |SC  |Seychelles                                |
|187       |SL  |Sierra Leone                              |
|188       |SG  |Singapore                                 |
|189       |SK  |Slovak Republic                           |
|190       |SI  |Slovenia                                  |
|191       |SB  |Solomon Islands                           |
|192       |SO  |Somalia                                   |
|193       |ZA  |South Africa                              |
|194       |GS  |South Georgia &amp; South Sandwich Islands|
|195       |ES  |Spain                                     |
|196       |LK  |Sri Lanka                                 |
|197       |SH  |St. Helena                                |
|198       |PM  |St. Pierre and Miquelon                   |
|199       |SD  |Sudan                                     |
|200       |SR  |Suriname                                  |
|201       |SJ  |Svalbard and Jan Mayen Islands            |
|202       |SZ  |Swaziland                                 |
|203       |SE  |Sweden                                    |
|204       |CH  |Switzerland                               |
|205       |SY  |Syrian Arab Republic                      |
|206       |TW  |Taiwan                                    |
|207       |TJ  |Tajikistan                                |
|208       |TZ  |Tanzania, United Republic of              |
|209       |TH  |Thailand                                  |
|210       |TG  |Togo                                      |
|211       |TK  |Tokelau                                   |
|212       |TO  |Tonga                                     |
|213       |TT  |Trinidad and Tobago                       |
|214       |TN  |Tunisia                                   |
|215       |TR  |Turkey                                    |
|216       |TM  |Turkmenistan                              |
|217       |TC  |Turks and Caicos Islands                  |
|218       |TV  |Tuvalu                                    |
|219       |UG  |Uganda                                    |
|220       |UA  |Ukraine                                   |
|221       |AE  |United Arab Emirates                      |
|222       |GB  |United Kingdom                            |
|223       |US  |United States                             |
|224       |UM  |United States Minor Outlying Islands      |
|225       |UY  |Uruguay                                   |
|226       |UZ  |Uzbekistan                                |
|227       |VU  |Vanuatu                                   |
|228       |VA  |Vatican City State (Holy See)             |
|229       |VE  |Venezuela                                 |
|230       |VN  |Viet Nam                                  |
|231       |VG  |Virgin Islands (British)                  |
|232       |VI  |Virgin Islands (U.S.)                     |
|233       |WF  |Wallis and Futuna Islands                 |
|234       |EH  |Western Sahara                            |
|235       |YE  |Yemen                                     |
|237       |CD  |Democratic Republic of Congo              |
|238       |ZM  |Zambia                                    |
|239       |ZW  |Zimbabwe                                  |
|242       |ME  |Montenegro                                |
|243       |RS  |Serbia                                    |
|244       |AX  |Aaland Islands                            |
|245       |BQ  |Bonaire, Sint Eustatius and Saba          |
|246       |CW  |Curacao                                   |
|247       |PS  |Palestinian Territory, Occupied           |
|248       |SS  |South Sudan                               |
|249       |BL  |St. Barthelemy                            |
|250       |MF  |St. Martin (French part)                  |
|251       |IC  |Canary Islands                            |
|252       |AC  |Ascension Island (British)                |
|253       |XK  |Kosovo, Republic of                       |
|254       |IM  |Isle of Man                               |
|255       |TA  |Tristan da Cunha                          |
|256       |GG  |Guernsey                                  |
|257       |JE  |Jersey                                    |
