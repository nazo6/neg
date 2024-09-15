# パーツ

Kicadのシンボル、フットプリントと実際に使うパーツの対応

## バッテリーケース

- KiCad中の情報

| 名前      | 値                                       |
| --------- | ---------------------------------------- |
| Ref       | BT1                                      |
| Symbol    | Device:Battery_Cell                      |
| Footprint | Battery:BatteryHolder_Keystone_2460_1xAA |

- 使用したライブラリの参照先

| 名前         | 値                                             |
| ------------ | ---------------------------------------------- |
| データシート | https://www.keyelco.com/product-pdf.cfm?p=1025 |
| 販売URL      | https://www.marutsu.co.jp/pc/i/10533103/       |

- 実際に使うパーツの情報

| 名前         | 値                                                        |
| ------------ | --------------------------------------------------------- |
| 型番         | BH-311-1P24                                               |
| データシート | https://cdn.ozdisan.com/ETicaret_Dosya/576276_7934662.pdf |
| 販売URL      | https://akizukidenshi.com/catalog/g/g100308/              |
| 備考         | 恐らく互換だと思う                                        |

## 昇圧DC-DCコンバータ

- KiCad中の情報

| 名前      | 値                                    |
| --------- | ------------------------------------- |
| Ref       | U3                                    |
| Symbol    | neg:AE-XCL103-3V3_Vertical            |
| Footprint | neg_footprints:AE-XCL103-3V3_Vertical |

- 実際に使うパーツの情報

| 名前         | 値                                                     |
| ------------ | ------------------------------------------------------ |
| 型番         | BH-311-1P24                                            |
| データシート | https://akizukidenshi.com/goodsaffix/AE-XCL103-3V3.pdf |
| 販売URL      | https://akizukidenshi.com/catalog/g/g116116/           |
| 備考         | ライブラリ不使用。細ピンヘッダ(0.8mm穴)                |

※付属ピンヘッダのデータシート:
https://akizukidenshi.com/goodsaffix/PHA-1x40SG_Color.pdf

## 74HC595 シフトレジスタ

- KiCad中の情報

| 名前      | 値                                   |
| --------- | ------------------------------------ |
| Ref       | BT1                                  |
| Symbol    | 74xx:74HC595                         |
| Footprint | Package_SO:SOIC-16_3.9x9.9mm_P1.27mm |

- 使用したライブラリの情報

| 名前         | 値                                             |
| ------------ | ---------------------------------------------- |
| データシート | http://www.ti.com/lit/ds/symlink/sn74hc595.pdf |

- 実際に使うパーツ

| 名前    | 値                                                          |
| ------- | ----------------------------------------------------------- |
| 型番    | 74HC595D,118                                                |
| 販売URL | https://jlcpcb.com/partdetail/Nexperia-74HC595D118/C5947    |
| 備考    | メーカーが違う同じ物だと思われる。JLCPCBでBasicに入っている |

## TRRSジャック

- KiCad中の情報

| 名前      | 値                                     |
| --------- | -------------------------------------- |
| Ref       | J1                                     |
| Symbol    | Connector_Audio:AudioJack4             |
| Footprint | PCM_marbastlib-xp-various:CON_MJ-4PP-9 |

- 実際に使うパーツ

| 名前    | 値                                           |
| ------- | -------------------------------------------- |
| 販売URL | https://akizukidenshi.com/catalog/g/g106070/ |
| 備考    | ライブラリと同じ型番の物が秋月で売ってる。   |

## LED_POWERスイッチ

参考: https://github.com/joric/nrfmicro/wiki/Components#rgb

LEDへの電力供給を遮断できるように、PMOSを配置する
