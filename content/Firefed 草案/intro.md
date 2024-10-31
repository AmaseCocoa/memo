# 作った理由
・ソーシャルネットワークに特化した連合の仕様が欲しい
・ActivityPubは(特に署名関連の) 実装が面倒すぎる
・興味 (そもそもこれに準拠する実装がFirefly (旧Holo, 元々Fireflyサーバー間でのデータ交換をできるだけ効率良く行うという意図もあったため)以外現れるとは思っていないので。)
## 考えていること
・ActivityPub実装との両立ができるように
	・例えばActivityPubのInboxのような物は`/.ffe/inbox`みたいな場所に置く
 ・webfingerは流用する？
 	・relがselfでtypeがapplication/ffe+jsonな感じにする
・nodeinfoはActivityPubのものと同じものを使う (ただし対応サーバーか識別するために必須にする可能性あり)
