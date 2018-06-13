更新方法（以更新到react-native0.55.4为例）
ls -A | grep -vE '^(\.git|buglist\.md)$' | xargs rm -rf
wget https://cdn.npm.taobao.org/promise/-/promise-7.3.1.tgz
tar -xf promise-*.tgz
cp -r package/. .
rm -rf package promise-*.tgz
根据bug列表和git历史在新的版本上进行修改
提交到github，修改项目依赖的提交版本
