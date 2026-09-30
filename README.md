# 鎭嬬埍鏃ヨ 路 闄堥湒 & 鏂囨枃

涓€浠藉熀浜庣害浼氳褰曞仛鎴愮殑闈欐€佺邯蹇靛皬绔欙細棣栧睆鎯呬功椋庛€佺浉鐖卞ぉ鏁扮粺璁°€佸彲绛涢€?鎼滅储鐨勬椂闂寸嚎銆?
**鍦ㄧ嚎璁块棶锛?* [https://caleb411.github.io/love-diary/](https://caleb411.github.io/love-diary/)  
**浠撳簱鍦板潃锛?* [https://github.com/Caleb411/love-diary](https://github.com/Caleb411/love-diary)

## 鏈湴鎵撳紑

鏈€绠€鍗曪細鍙屽嚮 `index.html` 鐢ㄦ祻瑙堝櫒鎵撳紑鍗冲彲銆?
鑻ュ凡瀹夎 Node.js锛屼篃鍙湪鏈洰褰曟墽琛岋細

```bash
npx --yes serve .
```

娴忚鍣ㄨ闂粓绔彁绀虹殑鍦板潃锛堜竴鑸槸 `http://localhost:3000`锛夈€?
Windows 涔熷彲鍦ㄦ湰鐩綍鍙抽敭銆岄€氳繃 Live Server 鎵撳紑銆嶏紙闇€ VS Code / Cursor 鎻掍欢锛夈€?
## 鐩綍缁撴瀯

```
love-diary/
鈹溾攢鈹€ index.html      # 鏁寸珯椤甸潰锛堝崟鏂囦欢锛屽惈鏍峰紡涓庢暟鎹級
鈹溾攢鈹€ SOURCE.md       # 椤圭洰鍘熷鏁版嵁锛堟亱鐖辨棩璁?Markdown锛?鈹溾攢鈹€ package.json    # 鏈湴棰勮鑴氭湰锛堝彲閫夛級
鈹溾攢鈹€ vercel.json     # Vercel 閮ㄧ讲閰嶇疆锛堝彲閫夛級
鈹溾攢鈹€ netlify.toml    # Netlify 閮ㄧ讲閰嶇疆锛堝彲閫夛級
鈹斺攢鈹€ README.md
```

## 閮ㄧ讲鏂瑰紡锛堜换閫夊叾涓€锛?
鏈珯鏄函闈欐€侀〉锛?*鍙戝竷鏍圭洰褰曞氨鏄湰鏂囦欢澶?*锛屽叆鍙ｄ负 `index.html`銆?
### 1. GitHub Pages锛堝厤璐癸級

1. 鏂板缓 GitHub 浠撳簱锛屾妸鏈洰褰曟帹涓婂幓  
2. 浠撳簱 **Settings 鈫?Pages**  
3. Source 閫?`Deploy from a branch`  
4. Branch 閫?`main`锛屾枃浠跺す閫?`/ (root)`  
5. 淇濆瓨鍚庣瓑寰?1锝? 鍒嗛挓锛岃闂細  
   `https://<鐢ㄦ埛鍚?.github.io/<浠撳簱鍚?/`

鑻ヤ粨搴撳悕鏄?`username.github.io`锛屽垯鐩存帴璁块棶 `https://username.github.io/`銆?
### 2. Vercel锛堟帹鑽愶紝鎷栨嫿鎴?CLI锛?
**缃戦〉鎷栨嫿锛?*

1. 鎵撳紑 [https://vercel.com/new](https://vercel.com/new)  
2. 鎶婃暣涓?`love-diary` 鏂囦欢澶规嫋杩涘幓  
3. 閮ㄧ讲瀹屾垚鍚庝細寰楀埌涓€涓?`*.vercel.app` 閾炬帴  

**鎴?CLI锛?*

```bash
npx vercel
```

鏈洰褰曞凡鍚?`vercel.json`锛屾寜闈欐€佺珯鐐瑰鐞嗐€?
### 3. Netlify

**鎷栨嫿锛?*

1. 鎵撳紑 [https://app.netlify.com/drop](https://app.netlify.com/drop)  
2. 鎷栧叆 `love-diary` 鏂囦欢澶? 
3. 鑾峰緱 `*.netlify.app` 閾炬帴  

**鎴栧叧鑱?Git锛?* 瀵煎叆浠撳簱鍚庯紝Publish directory 濉?`.`锛堟垨鐣欑┖锛夈€?
鏈洰褰曞凡鍚?`netlify.toml`銆?
### 4. Cloudflare Pages

1. Cloudflare Dashboard 鈫?Workers & Pages 鈫?Create 鈫?Pages  
2. 杩炴帴 Git 浠撳簱锛屾垨鐩存帴涓婁紶闈欐€佽祫婧? 
3. Build command 鐣欑┖锛孫utput directory 濉?`/` 鎴?`.`

## 鑷畾涔?
| 鎯虫敼浠€涔?| 鏀瑰摢閲?|
|---------|--------|
| 鏍囬 / 鍚嶅瓧 | `index.html` 閲?`.brand`銆乣.hero-title` |
| 琛ㄧ櫧璧峰鏃?| 鑴氭湰閲?`START_DATE`锛堝綋鍓嶄负 `2025-09-13`锛?|
| 绾︿細鏉＄洰 | 鑴氭湰閲?`diaries` 鏁扮粍 |
| 閰嶈壊 | `:root` CSS 鍙橀噺锛坄--rose`銆乣--rose-deep` 绛夛級 |

## 璇存槑

- 鏃犻渶鏋勫缓銆佹棤鍚庣渚濊禆  
- 瀛椾綋閫氳繃 Google Fonts 鍔犺浇锛岄娆℃墦寮€闇€鑱旂綉  
- 鐩哥埍澶╂暟鎸夋湰鍦版棩鏈熻嚜鍔ㄨ绠? 
