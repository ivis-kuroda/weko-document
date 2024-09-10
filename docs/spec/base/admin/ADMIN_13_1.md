### アクセス\_ロール

<!-- end list -->

  - > 目的・用途

本機能は、各ロールのシステムでのアクセスコントロールを管理する際に使用する機能である。

  - > 利用方法

【Administration \> ユーザー管理（User Management） \> アクセス：ロール（Access: Roles）画面】にて操作を行う。

  - > 利用可能なロール

<table>
<thead>
<tr class="header">
<th>ロール</th>
<th>システム<br />
管理者</th>
<th>リポジトリ<br />
管理者</th>
<th>コミュニティ<br />
管理者</th>
<th>登録ユーザー</th>
<th>一般ユーザー</th>
<th>ゲスト<br />
(未ログイン)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>利用可否</td>
<td>○</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>

  - > 機能内容

<!-- end list -->

  - 【アクセス：ロール（Access: Roles）画面】には以下のタブが表示される
    
      - 一覧（List）
    
      - 作成（Create）
    
      - フィルターを追加▼（Add Filter▼）
        
          - 一覧（List）タブ選択中のみ表示
        
          - 外観はタブだが機能としてはプルダウンメニュー
    
      - 選択▼（With selected▼）
        
          - 一覧（List）タブ選択中のみ表示
        
          - 外観はタブだが機能としてはプルダウンメニュー
    
      - 編集（Edit）
        
          - 一覧（List）タブ選択中は非表示
        
          - 一覧（List）タブの操作によって表示される
        
          - 編集（Edit）タブまたは詳細（Details）タブ選択中に表示
    
      - 詳細（Details）
        
          - 一覧（List）タブ選択中は非表示
        
          - 一覧（List）タブの操作によって表示される
        
          - 編集（Edit）タブまたは詳細（Details）タブ選択中に表示

  - 「一覧」（List）タブにて現在のシステムでのアクセスコントロールを表示する
    
      - 表示項目は以下の通りである
        
          - チェックボックス
        
          - アクション（閲覧・編集・削除を表すアイコン）
        
          - 「Role Name」
        
          - 「Action」
        
          - 「Argument」
        
          - 「Deny」
    
      - 「フィルターを追加▼」（Add Filter▼）ボタンをクリックすると、以下の追加可能なフィルターリストを表示し、フィルター名をクリックすると当該フィルタの入力エリアを追加する
        
          - フィルター名は以下の通りである
            
              - 「Role Name」
                
                  - フィルター方式の選択肢：含む（contains）、含まれていません（not contains）、等しい（equals）、等しくない（not equal）、空（empty）、一覧にある（in list）、一覧にない（not in list）
                
                  - 入力された文字列を使い、選択したフィルター方式で絞り込む
            
              - 「Action」
            
              - フィルター方式の選択肢：上記の「Role Name」と同じである
                
                  - 入力された文字列を使い、選択したフィルター方式で絞り込む
            
              - 「Argument」
                
                  - フィルター方式の選択肢：上記の「Role Name」と同じである
                
                  - 入力された文字列を使い、選択したフィルター方式で絞り込む
            
              - 「Deny」
                
                  - フィルター方式の選択肢：等しい（equals）、等しくない（not equal）
                
                  - 入力エリアではなく選択肢「はい」「いいえ」を使い、「はい」ならアクセス許可のコントロール、「いいえ」ならアクセス拒否のコントロールを絞り込む
        
          - 設定したフィルターは「適用」（Apply）ボタンを押下することで一覧に適用される
        
          - 「フィルターをリセット」（Reset filter）ボタンを押下すると、設定したフィルターがリセットされる
    
      - 「選択▼」（With selected▼）ボタンをクリックすると、以下の追加可能な機能（現在削除ボタンのみ）を表示する
        
          - レコードにチェックを入れない場合、「削除」（Delete）ボタンを押すと、エラーメッセージを表示する  
            メッセージ：  
            　日本語：「少なくとも一つのレコードを選択してください。」  
            　英語：「Please select at least one record.」
        
          - レコードにチェックを入れる場合、「削除」（Delete）ボタンを押すと、確認ダイアログを表示する  
            メッセージ：  
            　日本語：「選択したレコードを削除してもよろしいですか。」  
            　英語：「Are you sure you want to delete selected records?」
            
              - 「OK」ボタンを押すと、該当ロールを削除し、メッセージを画面上部に表示する  
                メッセージ：  
                　日本語：「レコード数＋レコードが正常に削除されました。」  
                　英語：「Record was successfully deleted.」
            
              - 「キャンセル」（Cancel）ボタンを押すと、確認ダイアログを閉じる
    
      - アクセスコントロール行にて目アイコンを押すと、該当アクセスコントロールの詳細情報を「詳細」（Details）タブに表示する
        
          - 表示項目：Role、Action、Deny、Argument
        
          - 「移動」（Filter）テキストボックスにテキストを入力すると、入力値が項目名またはその値に含まれている項目に絞り込んで表示する
    
      - アクセスコントロール行にて鉛筆アイコンを押すと、該当アクセスコントロールを「編集」（Edit）タブに表示し、アクセスコントロールの情報が編集できる
        
          - 入力情報とボタン操作は、後述の「作成」（Create）タブと同じである
    
      - アクセスコントロール行にて削除アイコンを押すと、該当アクセスコントロールを削除し、メッセージを画面上部に表示する  
        メッセージ：  
        　日本語：「レコード数＋レコードが正常に削除されました。」  
        　英語：「Record was successfully deleted.」

  - 「一覧」（List）から「作成」（Create）タブを押すと、「作成」（Create）タブに移動し、アクセスコントロールを新規作成できる
    
      - 入力情報は以下の通りである
        
          - 「Role」：必須項目  
            選択肢：システムに作成されたロール一覧
        
          - 「Action」：必須項目ではないがプルダウンメニューによって必ず１つ選択される  
            選択肢：「access\_actionsroles.action」から取得されている一覧
        
          - 「Argument」  
            255文字までの自由入力  
            255文字を超えると以下のエラーメッセージが表示される  
            メッセージ：  
            日本語：「フィールドは 255 文字を超えることはできません。」  
            英語：「Field cannot be longer than 255 characters.」
        
          - 「Deny」
    
      - 「保存」（Save）ボタンを押すと、設定されたアクセスコントロール内容をアクセスコントロール一覧に追加させ、メッセージをアクセスコントロール一覧に表示させる  
        メッセージ：  
        　日本語：「レコードが正常に作成されました。」  
        　英語：「Record was successfully created.」
        
          - アクセスコントロールをデータベースに保存する
            
              - テーブル名：「access\_actionsroles」
            
              - フィールド名：  
                ・「id」  
                ・「action」  
                ・「exclude」  
                ・「argument」  
                ・「role\_id」
    
      - ［保存してもう一つ追加（Save and Add Another）］ボタンを押すと、設定されたアクセスコントロール内容をロール一覧に追加させ、他のアクセスコントロールを追加設定可能とする  
        メッセージを画面上部に表示させる  
        メッセージ：  
        　日本語：「レコードが正常に作成されました。」  
        　英語：「Record was successfully created.」
    
      - ［保存して編集を続ける（Save and Continue Editing）］ボタンを押すと、設定されたアクセスコントロール内容をアクセスコントロール一覧に追加させ、該当アクセスコントロールの編集を続けることを可能とする  
        メッセージを画面上部に表示させる  
        メッセージ：  
        　日本語：「レコードが正常に作成されました。」  
        　英語：「Record was successfully created.」
    
      - ［キャンセル（Cancel）］ボタンを押すと、設定されたアクセスコントロール内容をアクセスコントロール一覧に追加せず、「一覧」（List）タブに戻る

  - v0.9.22でのデフォルトアクセスコントロールは以下の通りである
    
      - パス： <https://github.com/RCOSDP/weko/blob/v0.9.22/scripts/populate-instance.sh#L241-L338>

<!-- end list -->

  - > 関連モジュール

<!-- end list -->

  - invenio\_access（WEKOソース内にforkされていない）

<!-- end list -->

  - > 処理概要

<!-- end list -->

  - 本画面は、flask\_adminのModelViewを使っている。

  - 画面の設定をもとに、以下のようにaccess\_actionsrolesテーブルに保存する。
    
      - 「id」フィールド：画面上の入力によらない
    
      - 「action」フィールド：画面上の「Action」で選択されたもの
    
      - 「exclude」フィールド：画面上の「Deny」にチェックが入っていたらTrue、そうでなければFalse
    
      - 「argument」フィールド：画面上の「Argument」の入力値
    
      - 「role\_id」フィールド：accounts\_roleテーブルで、画面上の「Role」で選択されたものと「name」が一致するレコードの「id」フィールド

  - 各actionは、関数へのアノテーションでアクセス制御に利用する。

<!-- end list -->

  - > 更新履歴

<table>
<thead>
<tr class="header">
<th>日付</th>
<th>GitHubコミットID</th>
<th>更新内容</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><blockquote>
<p>2023/08/31</p>
</blockquote></td>
<td>353ba1deb094af5056a58bb40f07596b8e95a562</td>
<td>初版作成</td>
</tr>
</tbody>
</table>