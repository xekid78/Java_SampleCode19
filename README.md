# JavaMapDisplayIn2DArray
二次元配列で地図表示

## 処理
二次元配列を使っての地図の表示

## コード
```
public class Mapdisp {

	public static void main(String[] args) {
		String[][] areaMap = new String[20][20];
        	areaMap[0][0] = "城";
       		areaMap[5][17] = "町";
        	areaMap[19][19] = "町";
        	for (int i = 0; i < areaMap.length; i++) {
            		for (int j = 0; j < areaMap[i].length; j++) {
                	if (areaMap[i][j] == null) {
                		if (i % 2 == 0 || j % 3 == 0) {
                			areaMap[i][j] = "  ";
                		} else {
                			areaMap[i][j] = "森";
                		}
                	}
                	System.out.print(areaMap[i][j]);
            	}
            	System.out.println("");
        	}

	}

}
```

## 開発環境
| 開発ツール |  |
|:-|:-|
| OS | Windows10 |
| 統合開発環境(IDE) | Eclipse 4.7.0 Oxygen |
| 開発言語 | Java8 |
