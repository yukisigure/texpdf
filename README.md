# texpdf
texをpdfにする補助スクリプト 絶対パス対応
@texpdf -rtcq texfile


Usage: texpdf [(-q | -i)][-rtcfpn] texfile"
- [-q]:quiet platex logs; platexをバッチモードで実行(ログ出力を抑制)
- [-i]:ignore platex option; platexをオプション無しで実行
- [-r]:remove subfiles; texfileと同一ディレクトリのaux, div, log, tocを削除
- [-t]:twice compile; platexを2回実行(参照番号\\ref等を反映)
- [-c]:compression image; pdf内部の画像を圧縮し, ファイルサイズを縮小(表示ズレの可能性あり)
- [-f]:force compile; 強制的にpdfを生成(platexのエラーを無視) -q オプションと併用を推奨(read image error等に対応)
- [-x]:xtractbb; png, jpg, pdfのBounding Box情報を生成
- [-d]:create presence directry; 現在のディレクトリにpdfを生成
- [-n]:not open pdf; pdfを作成後自動で開かない

✳︎ ファイル名にスペースが入っている場合の-rの挙動を修正しました
