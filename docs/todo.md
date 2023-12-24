# ToDo

## 新しいアイテム・エンチャを追加する

時系列は上から下へ

### 星座の塔
490131#星座の印章#
490132#星座の印章(力)#
490133#星座の印章(体力)#
490134#星座の印章(集中)#
490135#星座の印章(創造)#
490136#星座の印章(魔力)#
490137#星座の印章(聡明)#
312022#天与の才#
312045#魔獣の爪牙#
312046#根源への到達#
312047#不滅の肉体#
312048#叡知の王冠#
312049#蒼穹の覇者#

### 拡張4次
650025#グレイシア風魔手裏剣#
300499#潜在解放(天帝I)#
312922#潜在解放(ハイパーノービスI)#
312923#潜在解放(ソウルアセティックI)#
312924#潜在解放(ナイトウォッチI)#
312925#潜在解放(蜃気楼&不知火I)#
312926#潜在解放(スピリットハンドラーI)#
311209#氷華の魔力(星帝I)#
311210#氷華の魔力(ソウルリーパーI)#
311211#氷華の魔力(リベリオンI)#
311212#氷華の魔力(影狼&朧I)#
311213#氷華の魔力(サモナーI)#
311214#氷華の魔力(サモナーII)#
810002#アドゥルテル・フィデス・ライフル#
810008#ウィワートゥス・フィデス・ライフル#
800014#グレイシアハンドガン#
590021#アドゥルテル・フィデス・メイス#
590023#ウィワートゥス・フィデス・メイス#
540023#アドゥルテル・フィデス・スターダストブック#
540045#ウィワートゥス・フィデス・スターダストブック#
550025#アドゥルテル・フィデス・ソウルスティック#
550064#ウィワートゥス・フィデス・ソウルスティック#
510032#アドゥルテル・フィデス・ダガー#
510033#ウィワートゥス・フィデス・ダガー#
550028#アドゥルテル・フィデス・フォックステイル#
550066#ウィワートゥス・フィデス・フォックステイル#
500050#グレイシアベーシックソード#
550070#グレイシアフォックステイル#

### 12月アップデート
400581#情熱あふれるラビットリボン#
400582#ウォルフライエ#
420302#りんりんニャンカーベル#
490471#リングオブアルテミス#
312916#スキル石(ブレッシングLv10)#
312917#潜在解放(インペリアルガードIII)#
312918#潜在解放(ウィンドホークIV)#
312919#潜在解放(トルバドゥール&トルヴェールI)#
15282#ウサギ柄のシャツ#
21063#ソリッドクレイモア#
610035#ウィキッドカタール#
620016#ウィキッドアックス#
640031#ソリッドスタッフ#
650019#プレジション風魔手裏剣#
650020#スクラップ風魔手裏剣#
700050#プレジションボウ#
300292#エクストラジョーカーカード#
300293#エルジェーベトカード#
300294#ジェニファーカード#
300295#ジェネラルオークカード#
300296#ジクラウスカード#
300297#ゴブリンキングカード#
800009#プレジションハンドガン#
800010#スクラップハンドガン#
810005#プレジションライフル#
810006#スクラップライフル#
820004#プレジションショットガン#
820005#スクラップショットガン#
830008#プレジションガトリング#
830009#スクラップガトリング#
840004#プレジショングレネード#
840005#スクラップグレネード#
26140#魔女のホウキ#
500044#ソリッドエッジ#
500045#ウィキッドブレード#
510051#ウィキッドダガー#
510054#フォーティファイドエッジ#
530023#ソリッドスピアー#
540041#ソリッドマニュアル#
540042#ウィキッドブック#
540043#リラプスブック#
550054#ソリッドワンド#
550055#ソリッドロッド#
550056#ウィキッドフォックステイル#
550057#フォーティファイドロッド#
550058#リラプスフォックステイル#
550059#フォーティファイドワンド#
560030#プレジションフィスト#
570028#プレジションリュート#
580028#プレジションホイップ#
590036#ウィキッドクロス#
312960#潜在解放(ハイパーノービスII)#

## 固定詠唱の定数減少効果を調べる

## 固定詠唱の割合カット効果を調べる

例えば foot.js に固定詠唱エンチャントに関する記述がある
foot.js は足装備ではなくて処理の footer を示している？

	//----------------------------------------------------------------
	// 「エンチャント　固定詠唱-70%」の、装備効果
	//----------------------------------------------------------------
	if (CardNumSearch(CARD_ID_ENCHANT_KOTEIEISHO_70)) {
		chkary.push(70);
	}

これは card.dat.js で定義されている

   	CARD_ID_ENCHANT_KOTEIEISHO_70 = 2145;
	[2145,99,"固定詠唱時間-70%","固定詠唱時間-70%。",0],

item.dat.js より雪花セットの固定詠唱-70%について

	[4974,100,0,0,0,0,0,0,0,0,"固定詠唱時間 - 70%",9,250,0],

itemset.dat.js ではこう定義されている
4968 = 雪花のローブ、4970 = 雪花のマフラー、4973  = 雪花のシューズ である

	[4974,4968,4970,4973],

まさか文字列から逆引きしてる？

## CTの定数減少効果を調べる

## 変動詠唱の割合カット効果を調べる
