<h3> Задание 1 </h3>
<br> 1. Найдите полный хеш и комментарий коммита, хеш которого начинается на aefea.
<br> aefead2207ef7e2aa5dc81a34aedf0cad4c32545
<br> 2. Какому тегу соответствует коммит 85024d3?
<br> git show 85024d3
<br> v0.12.23 
<br> 3. Сколько родителей у коммита b8d720? Напишите их хеши.
<br> git show b8d720
<br> 56cd7859e0 и 9ea88f22fc
<br> 4. Перечислите хеши и комментарии всех коммитов, которые были сделаны между тегами v0.12.23 и v0.12.24.
<br> git show v0.12.23, git show v0.12.24, git log --since="2020-03-05T20:56:10-07:00" --until "2020-03-19T15:04:05-07:00" --pretty=format:"%h - %cd - %s"
<br> 9d0c8c5970 - Thu Mar 19 10:40:58 2020 -0400 - Remove changelog entry for fix already in 0.12.24<br/>
51ea5d6b2f - Thu Mar 19 10:37:30 2020 -0400 - Merge pull request #24411 from hashicorp/alisdair/registry-retry-panic<br/> 
1c1df6dc50 - Thu Mar 19 10:20:10 2020 -0400 - registry: Fix panic when server is unreachable<br/> 
7d6d653b4f - Thu Mar 19 08:04:12 2020 -0400 - Update CHANGELOG.md<br/> 
5f313a65ad - Thu Mar 19 08:01:16 2020 -0400 - command: remove 0.12upgrade (#24403)<br/> 
109c4bf6ef - Wed Mar 18 14:20:03 2020 -0700 - website: Remove links to the getting started guide's old location<br/> 
420e22ece4 - Wed Mar 18 09:11:44 2020 -0400 - Update CHANGELOG.md<br/> 
8c7a44355b - Wed Mar 18 09:08:40 2020 -0400 - command: Fix bug when using terraform login on Windows<br/> 
fb7035ac3e - Wed Mar 18 09:07:58 2020 -0400 - Merge pull request #24364 from hashicorp/alisdair/013upgrade<br/> 
ed1aebbeda - Wed Mar 18 08:58:20 2020 -0400 - terraform: large refactor to use Provider from configs.Resource (#24396)<br/> 
176202b502 - Tue Mar 17 13:09:16 2020 -0700 - Remove provider listing<br/> 
3578a5d80a - Tue Mar 17 14:01:51 2020 -0400 - state: update local unlock err (#24320)<br/> 
a3529cb455 - Tue Mar 17 13:56:58 2020 -0400 - vendor: Fix checksum for github.com/coreos/etcd (#24343)<br/> 
8116b9c493 - Tue Mar 17 09:43:02 2020 -0400 - Merge pull request #24389 from hashicorp/jbardin/module-expansion-getting-there<br/> 
a8b9547e0d - Mon Mar 16 16:50:48 2020 -0400 - fixup states.Resource change throughout packages<br/> 
ef19fb6203 - Mon Mar 16 14:36:16 2020 -0400 - configs: attach provider fqn to Resource (#24382)<br/> 
3b0b29ef52 - Mon Mar 16 12:50:24 2020 -0400 - command: Add scaffold for 0.13upgrade command<br/> 
d905b990a5 - Mon Mar 16 11:16:23 2020 -0400 - s/GraphNodeResource/GraphNodeConfigResource/<br/> 
a7de3d07b8 - Mon Mar 16 11:16:23 2020 -0400 - cleanup from resource state mods<br/> 
ea51b790bc - Mon Mar 16 11:16:23 2020 -0400 - states.Resource needs to record its module too<br/> 
3729e6a705 - Mon Mar 16 11:16:23 2020 -0400 - update MaybeFixUpResourceInstanceAddressForCount<br/> 
f0e175a835 - Mon Mar 16 11:16:23 2020 -0400 - add AbsResource.Config() ConfigResource<br/> 
42f7beff31 - Mon Mar 16 11:16:05 2020 -0400 - Merge pull request #24296 from hashicorp/pselle/module-targetable<br/> 
e6bac359ed - Fri Mar 13 19:01:23 2020 -0400 - Missing ConfigResource checks in TargetContains<br/> 
e3ad9ffb77 - Fri Mar 13 09:19:27 2020 -0400 - added module targetting tests<br/> 
bf91bff2c8 - Fri Mar 13 09:08:42 2020 -0400 - TargetContains improvements<br/> 
076c540076 - Fri Mar 13 09:08:42 2020 -0400 - Add a test for whole module targeting<br/> 
7407fee9c2 - Fri Mar 13 09:08:42 2020 -0400 - Make modules targetable<br/> 
50077eabe9 - Fri Mar 13 09:08:26 2020 -0400 - Merge pull request #24362 from hashicorp/jbardin/module-expansion-some-more<br/> 
d65bd64955 - Thu Mar 12 15:58:25 2020 -0400 - incorporate addrs.ConfigResource<br/> 
9054716caf - Thu Mar 12 15:58:25 2020 -0400 - implement addrs.ConfigResource<br/> 
482ae66e18 - Thu Mar 12 14:54:47 2020 -0400 - minor cleanup<br/> 
946eda3f3c - Thu Mar 12 11:11:29 2020 -0700 - configs: Return diagnostics (almost) directly from ParseProviderSourceString<br/> 
a851566c56 - Thu Mar 12 11:11:29 2020 -0700 - tfdiags: Diagnostics.ToHCL<br/> 
1c78b26012 - Thu Mar 12 12:00:00 2020 -0400 - terraform: provider source test (#24342)<br/> 
4a1ec05092 - Wed Mar 11 14:52:15 2020 -0400 - comment fixes<br/> 
33464568e8 - Wed Mar 11 14:32:23 2020 -0400 - Merge pull request #24346 from hashicorp/jbardin/module-expansion-another-part<br/> 
e13eecbc5b - Wed Mar 11 14:19:52 2020 -0400 - finish provider ModuleInstance replacement<br/> 
98cfb51f27 - Wed Mar 11 11:21:45 2020 -0400 - convert /terraform to use new provider config<br/> 
856791ec7e - Wed Mar 11 11:10:02 2020 -0400 - Merge pull request #24331 from hashicorp/jbardin/module-expansion-in-part<br/> 
1252726cda - Wed Mar 11 10:31:41 2020 -0400 - update CHANGELOG.md<br/> 
f6221100ee - Wed Mar 11 10:28:12 2020 -0400 - Merge pull request #24149 from mlafeldt/fix-oss-state-locking<br/> 
8497adcb6e - Tue Mar 10 20:25:44 2020 -0400 - AbsProviderConfig to use addrs.Module<br/> 
fae5f9958d - Tue Mar 10 20:22:22 2020 -0400 - remove GraphNodeModuleInstance from Resource types<br/> 
68b500c5c7 - Tue Mar 10 17:25:11 2020 -0400 - remove abs addrs from NodeAbstractResource<br/> 
245296850b - Tue Mar 10 17:25:11 2020 -0400 - fix reference transformer comments<br/> 
ab9a2935ce - Tue Mar 10 17:25:11 2020 -0400 - implement NodePlannableLocal<br/> 
67e06f4fbe - Tue Mar 10 17:25:11 2020 -0400 - remove more UnkeyedInstanceShim<br/> 
87776913c6 - Tue Mar 10 17:25:11 2020 -0400 - nodeExpandModule doesn't need a Path() method<br/> 
a104ecb69d - Tue Mar 10 17:25:11 2020 -0400 - GraphNodeExpand is not used<br/> 
be2629d2f9 - Tue Mar 10 17:25:11 2020 -0400 - GraphNodeSubPath -> GraphNodeModuleInstance<br/> 
215f60d5cf - Tue Mar 10 17:25:11 2020 -0400 - remove module shims from module expansion nodes<br/> 
6ae9013c3f - Tue Mar 10 17:25:11 2020 -0400 - add addrs.Module.Equal<br/> 
bd9cfca794 - Tue Mar 10 17:25:11 2020 -0400 - rename GraphNodeSubPath -> GraphNodeModuleInstance<br/> 
b1df763541 - Tue Mar 10 17:25:11 2020 -0400 - remove UnkeyedInstanceShim from ref transformer<br/> 
521bdcc241 - Tue Mar 10 17:25:11 2020 -0400 - implement GraphNodeModulePath<br/> 
51bdcbb48c - Tue Mar 10 17:21:05 2020 -0400 - Merge pull request #24341 from hashicorp/jbardin/cbd-test-fix<br/> 
5901952882 - Tue Mar 10 16:32:22 2020 -0400 - command: tests should not leave dirs behind thank you (#24340)<br/> 
cb99dddb4d - Tue Mar 10 16:16:50 2020 -0400 - fix a flapping test involving CreateBeforeDestroy<br/> 
c7cc0afb80 - Tue Mar 10 14:43:57 2020 -0400 - Mildwonkey/ps schema (#24312)<br/> 
ca26efc5af - Tue Mar 10 14:10:38 2020 -0400 - Update CODEOWNERS<br/> 
7bd0071719 - Tue Mar 10 14:10:27 2020 -0400 - Update CODEOWNERS<br/> 
40f2511629 - Tue Mar 10 11:07:21 2020 -0700 - Merge pull request #24335 from hashicorp/cgriggs01-vmc-links<br/> 
822f608a3c - Tue Mar 10 08:59:20 2020 -0700 - [Website] vmc provider links<br/> 
add16fc67b - Mon Mar 9 15:57:14 2020 -0400 - jsonstate: sort child modules by address for consistency (#24329)<br/> 
ff3895ea26 - Mon Mar 9 14:56:30 2020 -0400 - Set Codecov threshold to 0.05% to avoid flicker<br/> 
654e880bb8 - Mon Mar 9 13:16:29 2020 -0400 - Merge pull request #24084 from hashicorp/jbardin/cbd-instance-state<br/> 
3a079b04db - Mon Mar 9 11:04:07 2020 -0400 - Change file permission ordering to avoid race condition<br/> 
b95daa87c8 - Mon Mar 9 10:24:29 2020 -0400 - Fix permissions of habitat provision's user.toml<br/> 
94d7236cd4 - Mon Mar 9 09:27:45 2020 -0400 - Merge pull request #24313 from hashicorp/alisdair/fix-coverage-blips-in-statemgr-filesystem<br/> 
b948856cbb - Mon Mar 9 11:27:33 2020 +0900 - fix typo<br/> 
a77d5032d3 - Sun Mar 8 15:10:38 2020 +0900 - improve s3.html.md<br/> 
1b5e2b70c6 - Fri Mar 6 15:37:02 2020 -0800 - Update CHANGELOG.md<br/> 
f54e2a62bf - Fri Mar 6 17:55:28 2020 -0500 - states: Fix coverage blips in statemgr/filesystem<br/> 
6118d22c1f - Fri Mar 6 08:33:44 2020 -0500 - terraform: refactor ProvidedBy() to return an addrs.ProviderConfig interface (#24295)<br/> 

<br> 5.Найдите коммит, в котором была создана функция func providerSource, её определение в коде выглядит так: func providerSource(...) (вместо троеточия перечислены аргументы).
<br> git grep --p "func providerSource" и git log -S "func providerSource"
<br> 5af1e6234a - Martin Atkins - Tue Apr 21 16:28:59 2020 -0700
<br> 6. Найдите все коммиты, в которых была изменена функция globalPluginDirs.
<br> git log -S globalPluginDirs --oneline
<br> 65c4ba7363 Remove terraform binary
125eb51dc4 Remove accidentally-committed binary
22c121df86 Bump compatibility version to 1.3.0 for terraform core release (#30988)
7c7e5d8f0a Don't show data while input if sensitive
35a058fb3d main: configure credentials from the CLI config file
c0b1761096 prevent log output during init
8364383c35 Push plugin discovery down into command package
<br> 7. Кто автор функции synchronizedWriters?
<br> git log -S synchronizedWriters
<br> Martin Atkins
