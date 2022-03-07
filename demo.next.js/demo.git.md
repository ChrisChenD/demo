
ChrisChen2050@outlook.com
Asdfrew!23

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


https://www.cloudsavvyit.com/14870/how-to-set-up-https-personal-access-tokens-for-github-authentication/

git config --local --unset credential.helper
git config --global --unset credential.helper


git config credential.helper store

git config --global user.email 'ChrisChen2050@outlook.com'
git config --global user.name 'Asdfrew!23'

ChrisChen2050@outlook.com
Asdfrew!23

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


https://www.cloudsavvyit.com/14870/how-to-set-up-https-personal-access-tokens-for-github-authentication/

git config --local --unset credential.helper
git config --global --unset credential.helper


git config credential.helper store


# 把目录上传到 git

# 先设置代理
export url='github.com/ChrisChenD/module_creator'
rm .git -rf
git init
git remote add origin https://$url
git checkout -b main
git add .;git commit -m '.';git push
git push -f --set-upstream origin main





# 安装 git 客户端
curl -fsSL https://cli.github.com/packages/githubcli-archive-keyring.gpg | sudo dd of=/usr/share/keyrings/githubcli-archive-keyring.gpg
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/githubcli-archive-keyring.gpg] https://cli.github.com/packages stable main" | sudo tee /etc/apt/sources.list.d/github-cli.list > /dev/null

sudo apt update
sudo apt install gh

# 注册用户名密码
gh auth login
## REF https://docs.github.com/en/get-started/getting-started-with-git/caching-your-github-credentials-in-git

# proxy:
git config --global https.proxy http://127.0.0.1:8989 # 无效
export https_proxy=127.0.0.1:8989 # 有效



Chris@out.Chen2050.look.Asd.com.frew!23
