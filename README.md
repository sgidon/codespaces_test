# codespaces_test

これはGithub Codespacesのテストです。
いろいろやってみます。

早速いくつか不具合見つけた

日本語入力で半角の「Codespaces」と入力すると「CodespacesCodespaces」と二回入力になりますね。
どういうことでしょう？

日本語の変換で、候補の選択ができない。変換リストはでてくるんだけどすぐに消えてしまう場合が多い。



```
codespace ➜ ~/workspace/codespaces_test (main ✗) $ df -h
Filesystem      Size  Used Avail Use% Mounted on
overlay          63G   11G   50G  17% /
tmpfs            64M     0   64M   0% /dev
tmpfs           2.0G     0  2.0G   0% /sys/fs/cgroup
shm              64M  8.0K   64M   1% /dev/shm
/dev/sdb1        29G  2.1G   27G   8% /usr/bin/docker
/dev/sda1        16G   45M   15G   1% /tmp
/dev/loop0       63G   11G   50G  17% /etc/hosts
tmpfs           394M  704K  393M   1% /run/docker.sock
tmpfs           2.0G     0  2.0G   0% /proc/acpi
tmpfs           2.0G     0  2.0G   0% /proc/scsi
tmpfs           2.0G     0  2.0G   0% /sys/firmware
codespace ➜ ~/workspace/codespaces_test (main ✗) $ df -h .
Filesystem      Size  Used Avail Use% Mounted on
/dev/loop0       63G   11G   50G  17% /home/codespace/workspace
```

50GBあるけど、全てのCodespacesで共通利用なのかな？

とりあえず、何か実装して公開してみよう。
A-FrameのHello Worldを貼り付けてみる。

お、Extensionにvimがあるぞ。これでかつる。

適当に実装して、githubのsettingからGithub Pagesの設定をONとすると、公開できた。

Githubだけでコーディングとサイト公開ができてしまうのはうれしいですね。
ちょっとレスポンスが遅いのが気になりますが、Betaが取れる頃にはDesktop環境と遜色ない
使い心地になっていることを期待。

