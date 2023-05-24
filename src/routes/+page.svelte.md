<!--
  Very long lines are allowed. You probably want to enable word wrap in your editor.
  This is just a spicy markdown file, don't be intimidated by the Svelte in the middle.
-->

<script>
  import Stopwatch from './Stopwatch.svelte'
</script>

<Stopwatch />

# Manjarno

<!--
> Manjaro is just Arch with an installer
-->
> Manjaro 只是有着系统安装界面的 Arch 而已。

<!--
Surely, right?
-->
当然了，哪里不是呢？

<!--
## Announcement
-->
## 声明

<!--
Hi, I've made a somewhat large inaccuracy with regard to Manjaro's alleged financial issues. [You can read from Phil himself here](https://github.com/EmeraldSnorlax/manjarno/issues/32). He was not purchaser of the laptop, nor was he the one to finally approve the decision.
-->
在 Manjaro 的资金问题方面我的描述出现了很大的偏差。[你可以阅读 Phil 本人的说明](https://github.com/EmeraldSnorlax/manjarno/issues/32)。笔记本电脑并不是他买的，而他也不是最终批准这个决定的人。

<!--
## Foreword
-->
## 前言

<!--
It's impossible to not make mistakes, especially with software. While it's tempting to mock every single mistake, that isn't really the point of this page.
Most things documented here to showcase a pattern of mistakes, with the events that were one-offs being things I (subjectively) feel are egregious enough warrant showing up here.
If you have any feedback or questions, or want to suggest changes, [open an issue or a pull request](https://github.com/EmeraldSnorlax/manjarno).
-->
要人不犯错是不可能的，尤其是在软件行业里。虽然对着每一个错误都嘲笑一番还是蛮诱人的，但本页面的目的并不在此。
在这里记载的大多数事情能展示出某种出错模式，而一些只发生过一次的事件则由我（主观）判定它是否足够异于寻常来决定是否把它们放到这里。
如果你有任何反馈或疑问，或者想提议一些改动，请[开一个 issue 或者是 pull request](https://github.com/EmeraldSnorlax/manjarno)。

<!--
A few others maintain similar resources to this -- you might also want to check out:
-->
有一些人也维护着类似本页面的资源——你可能也想去看看下面的内容：

- https://github.com/arindas/manjarno

<!--
## Security
-->
## 安全性

<!--
Manjaro has a track record of pretty poor security.
-->
Manjaro 的安全性不太好是有着纪录的。

<!--
### SSL Certificates
-->
### SSL 证书

<!--
[Manjaro has let their certificates expire twice!](https://redd.it/4inrut/)
-->
[Manjaro 已经让他们的证书过期两次了！](https://redd.it/4inrut/)

<!--
[No wait, thrice and counting.](https://web.archive.org/web/20220102232338/https://forum.manjaro.org/t/expired-certificate-for-iso-download-on-download-manjaro-org/96441)
-->
[待会儿等等，三次了，还在往上涨。](https://web.archive.org/web/20220102232338/https://forum.manjaro.org/t/expired-certificate-for-iso-download-on-download-manjaro-org/96441)

<!--
Four times! This one is a *little* better, as at [least they've set HSTS](./expiry-2022-08-17.png), but still, *[come on man](https://www.reddit.com/r/linuxquestions/comments/wqzrpl/did_manjaro_just_forget_to_renew_the_ssl/)*.
-->
四次了！这次*稍微*好一点，毕竟[他们至少设置了 HSTS](./expiry-2022-08-17.png)，但尽管如此，*[不是吧](https://www.reddit.com/r/linuxquestions/comments/wqzrpl/did_manjaro_just_forget_to_renew_the_ssl/)*。

<!--
[Five.](https://crt.sh/?q=66%3A16%3AD9%3A94%3AF4%3A7E%3A0F%3A87%3A1B%3A95%3A83%3A7D%3A7A%3ADE%3AB5%3A41%3A05%3A84%3A95%3A56) This time it was their archived forum. In fairness, they're [keeping up the trend of at least having HSTS on](./expiry-2022-11-06.png)? According to [this thread](https://forum.manjaro.org/t/am-i-the-only-one-getting-expired-certificate-warning-on-archived-forum-manjaro-org/126049), it seems like the server was abandoned.
-->
[第五次。](https://crt.sh/?q=66%3A16%3AD9%3A94%3AF4%3A7E%3A0F%3A87%3A1B%3A95%3A83%3A7D%3A7A%3ADE%3AB5%3A41%3A05%3A84%3A95%3A56)这次是他们的论坛归档。公道地说，他们[把趋势坚持了下去——至少开启了 HSTS](./expiry-2022-11-06.png)？根据[这个帖子](https://forum.manjaro.org/t/am-i-the-only-one-getting-expired-certificate-warning-on-archived-forum-manjaro-org/126049)，看起来这个服务器是被遗弃了。

<!--
The first time their certificate expired, they told their users to roll their clocks back as a fix:
-->
他们第一次证书过期时，他们让用户把自己的电脑时钟拨回去来解决问题。

https://web.archive.org/web/20150409040851/https://manjaro.github.io/expired_SSL_certificate/

<!--
> Seems we forgot to update our SSL certificate in time. [...] In time, please use followed workaround:
>
> open a terminal
>
> enter followed line: sudo date -s 2015-04-06 +09
>
> This will set back your system time to Mo 6. Apr 00:00:03 CEST 2015.
-->
> 看起来我们忘记及时更新我们的 SSL 证书了。 [...] 在此期间，请使用下面的临时应对办法：
>
> 打开终端
>
> 输入这行代码：sudo date -s 2015-04-06 +09
>
> 这会把你的系统时间设置回 Mo 6. Apr 00:00:03 CEST 2015。

<!--
### Holding packages back
-->
### 延迟软件更新

<!--
Holding back packages for two weeks can also cause security issues, but this issue is probably better addressed in the stability section.
--->
延迟两周再更新软件包也会导致安全问题，但这个问题大概在稳定性一节里讨论更好。

<!--
## Stability
--->
## 稳定性

<!--
I have used both Manjaro and Arch for a while, and have ironically had fewer problems with the stability of Arch than Manjaro. Manjaro would often require coaxing to get packages to install, which seems to defeat the purpose of using Manjaro, a supposedly more user-friendly alternative to Arch.
--->
Manjaro 和 Arch 两者我都用了好一会儿了，而讽刺的是我经历过的 Arch 的稳定性问题反而比 Manjaro 的要少。

<!--
You've probably seen across their resources that Manjaro holds Arch packages behind for two
weeks. Stability is stated as the reason for this, but that doesn't make much sense.
--->
你大概已经在他们的资源里得知了 Manjaro 比 Arch 的软件发布会慢两周。在其说明里这样做的原因是为了稳定性，但这没什么道理。

<!--
In practice, what this means is that software upgrades reach you later for seemingly
no reason. That means getting updates -- new features, security patches, bug fixes -- two whole weeks late. Aside from the obvious downside, it also causes a more insidious issue.
-->
实际上，这意味着你将更晚获得软件的更新，尽管看起来没什么正当理由。这意味着要晚两周才能获得软件的更新——包括了新特性、安全补丁和漏洞修复。除了这些明显的缺点，它还带来了一个潜在的问题。

<!--
### The AUR
-->
### AUR

<!--
I'm sure one of the reasons you're gravitating towards Manjaro is the AUR. Being able to run install scripts for anything sure sounds neat, right? Well, you need to be aware that you shouldn't trust the AUR in the same way you trust your distro's repos, as the scripts are user submitted. You should skim these scripts before running them to avoid running something malicious.
-->
我敢肯定你偏向于 Manjaro 的原因之一就是 AUR。能运行一切东西的安装脚本听起来挺不错，不是吗？那你需要当心了，你不应该像信任你的发行版的软件库一样信赖 AUR，因为那里的脚本是由用户上传的。为了避免运行一些恶意代码，你应该在运行脚本之前浏览一下代码。

<!--
Also, most of these scripts are written with the assumption that you aren't running a system
that's effectively two weeks out of date. This causes [partial upgrades](https://wiki.archlinux.org/title/System_maintenance#Partial_upgrades_are_unsupported). At best, that program won't install or work correctly and at worst can cause all kinds of issues on your system with no obvious way to fix it.
-->
另外，大多数这些脚本都假设你运行的系统不会是实际上两周都没更新过的。这会导致[部分的更新](https://wiki.archlinux.org/title/System_maintenance#Partial_upgrades_are_unsupported)。最乐观的情况下，程序会无法安装或者不正常运作，而最差的情况下，程序会导致你系统出现各种没有明显解决办法的问题。

<!--
That, and Manjaro *doesn't actually support* the AUR. Despite their [contradictory messages](https://web.archive.org/web/20220221092555/https://forum.endeavouros.com/t/is-aur-down-again/24287/9), Manjaro hides behind [blaming the users of pamac](https://web.archive.org/web/20220221090752/https://forum.manjaro.org/t/aur-please-restrain-yourself/103318). They provide insufficient warnings about the AUR and the potential risks, while providing a simplified interface for installing AUR packages via pamac. This is akin to letting someone with no briefing into a construction site. Sure, the heavy machinery might be quicker than using a shovel, but they are ultimately putting themselves in danger due to not being made aware of the consequences.
-->
就是这样，Manjaro *其实并不支持* AUR。尽管他们[传递出来与此相反的信息](https://web.archive.org/web/20220221092555/https://forum.endeavouros.com/t/is-aur-down-again/24287/9)，Manjaro 还是[把责任归到 pamac 的用户头上](https://web.archive.org/web/20220221090752/https://forum.manjaro.org/t/aur-please-restrain-yourself/103318)来遮掩。他们对于 AUR 和潜在风险的警告不足，却又通过 pamac 提供了安装 AUR 包的简化界面。这类似于让人未经培训就进入建筑工地。当然，挖掘机可能比用铲子更快，但用户仍然因为没有被告知所作行为的后果而把自己置于了险境。


<!--
To be clear, I'm not inherently against Manjaro using the AUR. However, it should be something to think about carefully. The AUR requires at least some level of awareness, *especially* on a distro that likes to hold its packages back and make arbitrary changes. If you can reconcile this contradictory ideology, then at the very least pamac should be more careful in how it presents the AUR.
-->
澄清一点，我并不完全反对 Manjaro 使用 AUR。但是，这应该是需要仔细思考的东西。AUR 至少需要一定程度上的相关认识，*尤其*是在一个喜欢把软件包更新延迟并随意变更的发行版上。如果你能够接受这种反对的思想的话，那 pamac 至少应该在它对 AUR 的呈现上更谨慎一点。

<!--
~~pamac, and by extension Manjaro, also isn't very polite to the AUR. But you can read about their DDoSes below...~~
-->
~~pamac 以及扩展到 Manjaro，也对 AUR 不太礼貌。但你可以在后面再读到它们的 DDoS……~~

<!--
### Rushing Asahi out the door
-->
### 把 Asahi 赶出门外

<!--
In their attempt to get Asahi Linux out (and support Apple Silicon) as soon as possible, they ended [pulling the latest PKGBUILD without talking to the devs](https://web.archive.org/web/20221208084616/https://twitter.com/marcan42/status/1576414477272387584). This has resulted in them shipping potentially broken kernels to end users.
-->
在他们尝试把 Asahi Linux 尽早赶走的途中，他们最终[没有和对面开发者沟通就把最新的 PKGBUILD 拉取了下来](https://web.archive.org/web/20221208084616/https://twitter.com/marcan42/status/1576414477272387584)。这导致了他们把可能有问题的内核递送给了用户。

<!--
Still though, that's besides the main problem. It was [only about 3 days ago this video came out](https://www.youtube.com/watch?v=k0cnMUroMlQ), in which a DE is working for the first time. Not only is it still in a state far from prime-time, but compounded with the tweet above they didn't even bother trying to speak with the devs of the project about its current state.
-->
尽管如此，这还不是最主要的问题。这件事[是在这段视频出现之后的仅约三天后发生的](https://www.youtube.com/watch?v=k0cnMUroMlQ)（视频内容是桌面环境第一次能够运作了）。这不仅仅离递送“黄金档”还远得很，而且结合上面的推特来看他们甚至都懒得尝试去和项目的开发者沟通一下了解一下项目的当前状况。

<!--
## Management
-->
## 管理

<!--
### Funding
-->
### 资金

<!--
**This section is inaccurate, and left here for transparency's sake. [Read more here.](https://github.com/EmeraldSnorlax/manjarno/issues/32)**
-->
**本节内容并不精确，只是为了透明度而放在这里。[在这里了解更多。](https://github.com/EmeraldSnorlax/manjarno/issues/32)**

<!--
~~Manjaro has had a controversy with their treasurer. Phillip Muller (Manjaro team lead) had purchased a laptop for €2000, and the treasurer asked to clarify his purchase. [This ultimately led to the treasurer being removed.](https://redd.it/hxp3zi) Isn't the whole point of a treasurer to ensure fair and efficient use of donation funds?~~
-->
~~Manjaro 和他们的一个财务管理有过一个冲突。Phillip Muller（Manjaro 的团队领头）用 2000 欧元买了一台笔记本电脑，而财务管理请求对购买作出解释。[这最终导致了这个财务管理的免职。](https://redd.it/hxp3zi)财务管理不就是为了保证捐赠资金的公平、有效使用而存在的吗？~~

<!--
## Poor QA
-->
## QA 差

<!--
### DDoSing the AUR
-->
### 对 AUR 的 DDoS

<!--
Manjaro's AUR helper, pamac, shipped a version with a bug on 2020-04-26 that accidentally sent thousands
of requests to the AUR per user. This rendered the AUR offline for *all* users across
every Arch-based distro for a few hours.
-->
Manjaro 的 AUR 工具程序 pamac 在 2020-04-26 递送了有漏洞的一个版本，意外地让每名用户分别向 AUR 发送了成千的请求。在几小时内，这让 AUR 直接对*所有*基于 Arch 的发行版的用户来说变得无法访问了。

* https://www.reddit.com/r/archlinux/comments/mz3biz/is_the_aur_down_for_everyone/
* https://gitlab.manjaro.org/applications/pamac/-/issues/1017

<!--
### and again...
-->
### 再次……

<!--
On 2021-10-14, Manjaro once again shipped a bad version of pamac, resulting in pamac being
blocked again. This may have been the cause for the day's earlier outage.
-->
在 2021-10-14，Manjaro 又再次递送了 pamac 的有问题的一个版本，导致 pamac 再次被 AUR 屏蔽。这可能也可以解释当天更早的时候的 AUR 断线。

* https://www.reddit.com/r/linux/comments/q85t8n/pamac_manjaros_package_manager_gui_has_been/

* https://gitlab.manjaro.org/applications/pamac/-/issues/1135

<!--
While these incidents were in no way intentional, it highlights the poor QA testing that Manjaro performs. This has happened on two separate occasions in less than two years.
-->
虽然这些事故肯定不是故意而为的，但这也足够显示 Manjaro 所展示出的较差的 QA（质量保证）了。这种事情在两年内发生了两次。

<!--
## Miscellaneous
-->
## 杂项

<!--
[Their system update script used to run `rm` on the lockfile mid-transaction.](https://gitlab.manjaro.org/packages/core/manjaro-system/blob/3b806753e245b7ec7e18bb674e916e28d751a429/manjaro-update-system.sh#L45) The lockfile is in place to prevent multiple instances of pacman from trying to alter the package database at the same time. Sometimes, when pacman is interrupted, a stale lockfile can remain. In this case, removing the lockfile is a common troubleshooting step. However, you should only do that when you are **absolutely certain** there are no other pacman instances running. Manjaro's script used to do this silently without checking for other instances.
-->
[他们的系统更新脚本曾经对事务的锁文件使用了 `rm` 命令。](https://gitlab.manjaro.org/packages/core/manjaro-system/blob/3b806753e245b7ec7e18bb674e916e28d751a429/manjaro-update-system.sh#L45)锁文件是用来防止多个 pacman 同时尝试修改软件包数据库的。有些时候，pacman 被打断了的时候会残留一个锁文件。这种情况下，移除锁文件是很常见的检修步骤。但是，你应该*再三确保*没有其它的 pacman 在运行的时候才这样做。而 Manjaro 的脚本之前并没有检查有没有其它 pacman 而是直接进行。

---

<!--
## What should I use instead?
-->
## 作为替代，我应该用什么？

<!--
~~I am in no way affiliated with these projects.~~
-->
~~我并不隶属于这些项目。~~

<!--
* [Arch already has an installer.](https://github.com/archlinux/archinstall)
* [EndeavourOS](https://endeavouros.com/) seems to be what Manjaro is going for -- just rightly done as far as I can tell. That said, using an Arch derivative is still a bit questionable in my view. The main excuse for doing so (lack of an automated installer) doesn't apply anymore as Arch ships with `archinstall`. However, EndeavourOS has a GUI installer, which should be much more approachable, and offers many more configurations to choose from out of the box than `archinstall`.
-->
* [Arch 已经有一个系统安装器了。](https://github.com/archlinux/archinstall)
* [EndeavourOS](https://endeavouros.com/)看起来是 Manjaro 想要成为的样子——只是在我知道的范围内做得比 Manjaro 更对头一些。虽然这么说，在我看来，用 Arch 的衍生版系统还是有一些值得提起疑问的地方。这样做的主要理由（缺少自动化系统安装工具）已经不成立了，毕竟 Arch 已经递送了 `archinstall`。但是 EndeavourOS 有着对用户更友好一些的图形化的系统安装界面，也默认提供了比 `archinstall` 多很多的配置，任君选择。

<!--
Once again though, I'd like to reiterate that Arch already ships with a reasonably friendly installer.
-->
但我还是想要再说一遍，Arch 已经有一个相对友好的系统安装器了。

<!--
## Quick things
-->
## 简短说明

<!--
I know what I've written here can be seen as inflammatory, but that's not really what this page is for. This resource is to quickly have something to point to the next time someone says "should i use manjaro??" in a chat room.
-->
我知道我这里写的东西看起来有煽动性，但本页面的目的并不在此。这里的资源主要是为了下次在聊天室里有人问“我应该用 manjaro 吗？？”的时候你可以直接让人家读链接里的内容。

<!--
Maintaining a distro is commendable, and that alone takes credit. However, I'd rather not have
your time (and others, when Manjaro inevitably breaks, and you need to ask for help) wasted,
trying to figure out the odd quirks and issues that Manjaro causes.
-->
维护一个发行版令人钦佩，真的仅此都已经值得称道了。但是，我真的不希望你（以及别人，在 Manjaro 不可避免地坏掉然后你去找别人帮忙的时候）把时间浪费在 Manjaro 导致的各种奇怪问题上。

<!--
[Source code under BSD-3 Clause.](https://github.com/EmeraldSnorlax/manjarno)
-->
[源码在 BSD-3 Clause 下发布。](https://github.com/EmeraldSnorlax/manjarno)
