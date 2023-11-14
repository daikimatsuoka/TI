# 2重ハッシュの取り出し方
・ハッシュ自体はその値に対応するキーを指定
・2重ハッシュのキーを取得するためには取得するキーを取得するデータまで連続して指定
すべてのデータを取り出したいので上記をデータの数だけ繰り返す

```ruby
user_data = [
  {user: {profile: {name: 'George'}}},
  {user: {profile: {name: 'Alice'}}},
  {user: {profile: {name: 'Taro'}}},
 ]

user_data.each do |user|
  puts user[:user][:profile][:name]
end
