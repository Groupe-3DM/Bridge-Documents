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
|country_id|iso2|
|----------|----|
|1         |AF  |
|2         |AL  |
|3         |DZ  |
|4         |AS  |
|5         |AD  |
|6         |AO  |
|7         |AI  |
|8         |AQ  |
|9         |AG  |
|10        |AR  |
|11        |AM  |
|12        |AW  |
|13        |AU  |
|14        |AT  |
|15        |AZ  |
|16        |BS  |
|17        |BH  |
|18        |BD  |
|19        |BB  |
|20        |BY  |
|21        |BE  |
|22        |BZ  |
|23        |BJ  |
|24        |BM  |
|25        |BT  |
|26        |BO  |
|27        |BA  |
|28        |BW  |
|29        |BV  |
|30        |BR  |
|31        |IO  |
|32        |BN  |
|33        |BG  |
|34        |BF  |
|35        |BI  |
|36        |KH  |
|37        |CM  |
|38        |CA  |
|39        |CV  |
|40        |KY  |
|41        |CF  |
|42        |TD  |
|43        |CL  |
|44        |CN  |
|45        |CX  |
|46        |CC  |
|47        |CO  |
|48        |KM  |
|49        |CG  |
|50        |CK  |
|51        |CR  |
|52        |CI  |
|53        |HR  |
|54        |CU  |
|55        |CY  |
|56        |CZ  |
|57        |DK  |
|58        |DJ  |
|59        |DM  |
|60        |DO  |
|61        |TL  |
|62        |EC  |
|63        |EG  |
|64        |SV  |
|65        |GQ  |
|66        |ER  |
|67        |EE  |
|68        |ET  |
|69        |FK  |
|70        |FO  |
|71        |FJ  |
|72        |FI  |
|74        |FR  |
|75        |GF  |
|76        |PF  |
|77        |TF  |
|78        |GA  |
|79        |GM  |
|80        |GE  |
|81        |DE  |
|82        |GH  |
|83        |GI  |
|84        |GR  |
|85        |GL  |
|86        |GD  |
|87        |GP  |
|88        |GU  |
|89        |GT  |
|90        |GN  |
|91        |GW  |
|92        |GY  |
|93        |HT  |
|94        |HM  |
|95        |HN  |
|96        |HK  |
|97        |HU  |
|98        |IS  |
|99        |IN  |
|100       |ID  |
|101       |IR  |
|102       |IQ  |
|103       |IE  |
|104       |IL  |
|105       |IT  |
|106       |JM  |
|107       |JP  |
|108       |JO  |
|109       |KZ  |
|110       |KE  |
|111       |KI  |
|112       |KP  |
|113       |KR  |
|114       |KW  |
|115       |KG  |
|116       |LA  |
|117       |LV  |
|118       |LB  |
|119       |LS  |
|120       |LR  |
|121       |LY  |
|122       |LI  |
|123       |LT  |
|124       |LU  |
|125       |MO  |
|126       |MK  |
|127       |MG  |
|128       |MW  |
|129       |MY  |
|130       |MV  |
|131       |ML  |
|132       |MT  |
|133       |MH  |
|134       |MQ  |
|135       |MR  |
|136       |MU  |
|137       |YT  |
|138       |MX  |
|139       |FM  |
|140       |MD  |
|141       |MC  |
|142       |MN  |
|143       |MS  |
|144       |MA  |
|145       |MZ  |
|146       |MM  |
|147       |NA  |
|148       |NR  |
|149       |NP  |
|150       |NL  |
|151       |AN  |
|152       |NC  |
|153       |NZ  |
|154       |NI  |
|155       |NE  |
|156       |NG  |
|157       |NU  |
|158       |NF  |
|159       |MP  |
|160       |NO  |
|161       |OM  |
|162       |PK  |
|163       |PW  |
|164       |PA  |
|165       |PG  |
|166       |PY  |
|167       |PE  |
|168       |PH  |
|169       |PN  |
|170       |PL  |
|171       |PT  |
|172       |PR  |
|173       |QA  |
|174       |RE  |
|175       |RO  |
|176       |RU  |
|177       |RW  |
|178       |KN  |
|179       |LC  |
|180       |VC  |
|181       |WS  |
|182       |SM  |
|183       |ST  |
|184       |SA  |
|185       |SN  |
|186       |SC  |
|187       |SL  |
|188       |SG  |
|189       |SK  |
|190       |SI  |
|191       |SB  |
|192       |SO  |
|193       |ZA  |
|194       |GS  |
|195       |ES  |
|196       |LK  |
|197       |SH  |
|198       |PM  |
|199       |SD  |
|200       |SR  |
|201       |SJ  |
|202       |SZ  |
|203       |SE  |
|204       |CH  |
|205       |SY  |
|206       |TW  |
|207       |TJ  |
|208       |TZ  |
|209       |TH  |
|210       |TG  |
|211       |TK  |
|212       |TO  |
|213       |TT  |
|214       |TN  |
|215       |TR  |
|216       |TM  |
|217       |TC  |
|218       |TV  |
|219       |UG  |
|220       |UA  |
|221       |AE  |
|222       |GB  |
|223       |US  |
|224       |UM  |
|225       |UY  |
|226       |UZ  |
|227       |VU  |
|228       |VA  |
|229       |VE  |
|230       |VN  |
|231       |VG  |
|232       |VI  |
|233       |WF  |
|234       |EH  |
|235       |YE  |
|237       |CD  |
|238       |ZM  |
|239       |ZW  |
|242       |ME  |
|243       |RS  |
|244       |AX  |
|245       |BQ  |
|246       |CW  |
|247       |PS  |
|248       |SS  |
|249       |BL  |
|250       |MF  |
|251       |IC  |
|252       |AC  |
|253       |XK  |
|254       |IM  |
|255       |TA  |
|256       |GG  |
|257       |JE  |



