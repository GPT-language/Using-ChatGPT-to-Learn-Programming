## 前言


ChatGPT的功能只是回答问题，但使用起来却绝非看上去那么简单。举例来说，相比问“X是什么”，问“X是什么，请从基本原理进行解释”会得到更详细更全面的信息。相比问“请给我布置一些作业？”，问“请给我布置一些作业帮助我更好地理解和使用X，布置的作业按顺序应该由浅到深，由简单到难”得到的回答会更适用。学习如何将ChatGPT应用于编程学习，本质上就是学习如何更好地提问，使得ChatGPT在回答相关问题时能够准确且全面。



<details>
<summary> <strong> 使用ChatGPT学习编程的优势</summary></strong>



#### ChatGPT能够明显提高学习效率
可以将弄懂一个知识点所耗费的时间分为两部分：

1. 用于找到解答的时间

2. 用于理解解答的时间
 
ChatGPT将（1）和（2）所需的时间缩短到一个惊人的程度，特别是（1）部分。在ChatGPT之前，我们需要耗费大量的时间在（1）中。大家可以回想自己在ChatGPT之前为找到某个问题的解答的经历，有时候我们甚至可能在这上面花费数小时乃至数天，而ChatGPT不需要一分钟就能解决（更复杂的问题则需要多次交互，但花费的时间也要少得多得多）。而在（2）中，ChatGPT也能帮助你迅速理解解答并且针对对你的任何疑惑做出解答。


以前我们也许需要花费数个小时甚至数天来寻找答案，而理解答案的过程却不需要十分钟，现在有了ChatGPT，我们可以将整个过程——从寻找到理解答案——都缩短到5分钟。

#### ChatGPT能够降低学习的难度
**ChatGPT对于知识点的解释是动态的**，这一点是它和搜索引擎、书籍和其它知识获取方式的本质差异。同样一个知识点，如果出现在书或搜索引擎上，它的解释是已经固定的，它不会因为你看不懂而修改一个字，而如果出现在ChatGPT，你可以说“我看不懂，请解释得更详细一点”，可以说”我看不懂英文，请使用中文解答“，可以说“请尝试向一个完全没有这方面知识的人解释这个知识点”。

此外**ChatGPT还能够基于单个知识点无限扩展、延伸，帮助你理解各个知识点之间的关系，将知识点放入整个知识体系和实践中**。

#### ChatGPT能够降低学习的成本

最直接的，ChatGPT免去了购买大部分书籍的花费。我们只需要一个网站，或者只是一张完备的学习路径图，接下来的都可以交给ChatGPT。只有在学习到一定深度后，我们才需要特别购买一些书籍来补充欠缺。

ChatGPT免去了培训的费用。没有任何老师能够像ChatGPT这样，全天无休等待你的提问，耐心、专业，从不感到厌烦。

唯一且非常值得的费用也许是ChatGPT Plus的会员费用，每月20＄，绝对物超所值。

</details>


<details>
<summary> <strong> ChatGPT的一些特性</summary></strong>
 
在正式开始学习之前，有必要先简单介绍一下ChatGPT的一些特性，利用好这些特性能够帮助你更正确地设计你的问题，从而提高ChatGPT的回答质量。

#### ChatGPT的回答质量取决于提问质量
不同提问方式得到的答案质量差异是巨大的。比如我之前提到的，同样一个知识点，如果你只是普通询问“是什么”，那给出来的回答就会比较简单，有时候无法满足你对这个知识点应该达到的掌握程度。但是如果你问“X是什么？请从底层原理进行解释”，那么ChatGPT给出的答案就会详细得多。我们需要根据我们所问问题的情境，设计出适合该类问题的提问方式，这样才能得到质量更好的回答。


#### ChatGPT的答案并非一蹴而就
ChatGPT并不是一键给出正确答案，它是在与你不断交互的过程中才慢慢形成一个较为正确的回答，并且这个回答还能继续根据你的反馈进行修正。这就也是说，在绝大多数情况下，如果它的回答不能满足你的需求，你应该继续补充条件或者尝试修改自己的提问方式，并且将代码的结果也反馈给它。这样经过多轮的交互后，相比最初，ChatGPT给你的回答会清晰有效得多。当然，可能直到最后ChatGPT给出的结果也并不能让你满意，这就要说到下一个特点。

#### 使用ChatGPT并非只是为了获得正确答案
使用ChatGPT来完成一个任务和使用ChatGPT来学习是两回事。在前者的情境下，你会要求ChatGPT能够尽可能地正确且迅速地完成你的需求，但在后者的情境下，你要做的是从ChatGPT中的回答中学习到你要学习的内容。ChatGPT给予你的实现某个方法的代码可能是错误的，但是你可以把报错信息反馈给它让它改正，也可以让它解释这段代码，让它告诉你是如何实现这段代码的。总之错误很正常，你需要做的是从错误中学习。最理想的情况是你在它的教导下，从它的错误和自己的错误中学习，最后与它合力写出正确的代码。

</details>


## 使用ChatGPT帮助学习编程

基于以上特性和个人使用经验，我将**在学习过程中可能会遇到的不同问题的有效提问方式**总结成一套指令集，我将其命名为“有效指令集”，并基于该指令集设计出一套系统的学习模式。接下来我会举例一一介绍这些有效指令的使用方式，并在这个过程中展现这套学习模式是如何运作的。不过在介绍这些指令之前我先引入一个简单工具。
<details>
<summary> <strong> Quicker</summary></strong>

网站：https://getquicker.net/Download

Quicker是一款 Windows 平台上的快捷操作工具，可以帮助我们更快速、更方便地完成我们需要的操作。比如同样询问A/B/C/D知识点，不需要花费时间每次都输入““A/B/C/D是什么？请从底层原理进行解释”，只需要将指令"X是什么？请从底层原理进行解释“输入Quiker中，然后我们选中A/B/C/D，然后使用Quiker一键替换掉X即可。将所有指令都输入到Quicker后，能减少我们在输入上浪费的时间。使用其它有类似功能的快捷操作工具亦可。

[示例视频1]( https://www.bilibili.com/video/BV1rM4y1B7rw/?share_source=copy_web&vd_source=517d066e1daeca655783363f1e449202)

**如有需要，后续将发布如何使用Quicker录制指令的视频**
</details>

<details>
<summary> <strong> 有效提问1：想要深入了解和使用X，我需要学习哪些内容？并且告诉我正确的学习步骤</summary></strong>


接下来以”哈希搜索算法“（此处的”哈希搜索算法“更常见的中文叫法应为哈希查找算法，ChatGPT能够理解，不影响回答的准确性）为例对ChatGPT做出第一个提问。对于一个陌生的知识点，许多人的第一个提问往往是“X是什么”，但这并不是一个有效提问，ChatGPT给出的答案往往也并不能让人满意。而在使用另外一种更合理、有效的提问方式后，给出的答案立即得到改善。读者可以做出对比，注意在不同的询问方式下ChatGPT给出答案的不同。

![Pasted image 20230316162630](https://user-images.githubusercontent.com/69788237/227186142-4006eb4c-2b8f-4ac3-916b-7ac0e7cb562c.png)
![Pasted image 20230316162643](https://user-images.githubusercontent.com/69788237/227186487-efcd20b5-71b9-490e-be25-9be4f0461c04.png)

>因为只是示例，考虑到响应速度，使用的model是GPT-3.5。使用GPT-4答案会更准确，但使用体验未必更好。

哪种提问方式更好一目了然。

**任何一个知识点它不是独立的，它是其它知识点的基础，它自身也由很多更底层的知识点构成，当我们学习一个知识点我们不能直接问它是什么，这样提问得出的回答很可能是不全面，甚至无效的。**了解一个知识点，特别是位于知识体系中较为高层的知识点，必须也得了解与它相关的更底层的知识点，有效提问1的作用就是这个。


<details>
<summary> <strong> 使用GPT-3.5还是4.0</summary></strong>


同一个问题，ChatGPT4.0的回答：

![Pasted image 20230316185135](https://user-images.githubusercontent.com/69788237/227186910-32cc5bc9-3942-4893-b767-950e76369807.png)

对比两个回答，可以发现两者在对于知识点的回答上其实是相似的，所以在学习概念和知识点上其实可以优先选择响应速度快得多的GPT-3.5。什么时候优先使用GPT-4，这我也会在下文用到时指出。
</details>
</details>

<details>
<summary> <strong> 对ChatGPT回答的分析</summary></strong>


在有效提问1的回答中，ChatGPT给出了所有关于该知识点我们需要学习的内容，接下来我们要捋清楚关于这些学习内容，我们是要学习关于它们的什么，我们要以怎样的方式来学习，这直接决定了我们应该如何设置我们的提问。

一般来说，关于某个知识点，我们要学习以下内容：

1.是什么
2.为什么
3.真实的应用场景是什么
4.怎么做
5.做得是否正确，哪里错误，如何修改

1、2是为了从概念上理解知识点，3是为了从应用场景上理解这个知识点的作用（如果不了解这一点，很多知识点的学习会变得很枯燥也很抽象），4、5是为了实践操作。

缕清以上内容后，我们就可以根据不同的学习内容设计不同的有效提问。从概念上、从应用场景上、从实践上，三个不同的视角，设计提问时需要不同的侧重点。

接下来我们就只需要根据以上步骤对ChatGPT回答的学习进行学习即可，这里我将使用我发现的另一个**有效指令：X的相关内容**。在通过指令”什么是X？请从底层原理进行解释“提问之前，我们可以先使用这个有效指令来进行一个总体和广度上的认识。
</details>



<details>
<summary> <strong> 有效提问2：X的相关内容</summary></strong>



比如对“哈希函数的设计和实现”：

![Pasted image 20230316165421](https://user-images.githubusercontent.com/69788237/227187051-1142eeb0-26b8-457d-af1c-2248762a3a9e.png)

如果你对以上内容不满意，可以继续追问。

![Pasted image 20230316185636](https://user-images.githubusercontent.com/69788237/227187197-ffd97b6e-8fc4-4212-95e1-ab8ee513e245.png)

**对于基础的知识点，如果觉得不对劲可以对比Google和书。就我的经验来看，ChatGPT很少在比较宽泛、通用、基础的知识点上犯错（当然也很可能只是犯错了但我不知道而已，这一点请在使用时自己斟酌）。**
</details>


<details>
<summary> <strong> 有效提问3：什么是X？请从底层原理进行解释</summary></strong>


有效提问2是为了对X做出一个总的介绍，扩展和延申关于X的内容，这是广度上的认识。想要完全理解一个概念，特别是计算机中一些关键的概念，需要足够深度的认识，这就是有效提问3的作用。

![Pasted image 20230316193116](https://user-images.githubusercontent.com/69788237/227192986-2d6bba22-2d41-474b-93d5-9e537f1d66cb.png)

从回答中我们可以发现，虽然相比直接问“是什么”更加详细，但是并没有谈到什么“底层原理”。**这是因为“底层原理”这个表述其实并不适用于“哈希搜索算法”这个概念，”哈希搜索算法“的重要其实不在于它是什么，它而在在于如何实现及实现的原理**。对于这类情况，我们还需要追求一个有效提问4。


<details>
<summary>什么时候适用“底层原理”</summary>
![Pasted image 20230316194256](https://user-images.githubusercontent.com/69788237/227193310-32a74232-ba94-44d2-9fe0-c9f7aa51743a.png)

![Pasted image 20230316194356](https://user-images.githubusercontent.com/69788237/227193336-6b140a53-41ba-47a2-bffe-0fadcae11226.png)

当我们学习操作系统或任何底层原理时，这个提问的作用便十分明显。

</details>
</details>

<details>
<summary> <strong>  有效提问4：X是如何实现的？请告诉我它的实现原理</strong></summary>


![Pasted image 20230316195201](https://user-images.githubusercontent.com/69788237/227193934-c1c4a426-2c46-4da2-bcb9-72cad03ad683.png)

![Pasted image 20230316195214](https://user-images.githubusercontent.com/69788237/227194083-5880febf-6059-4d05-8314-ba9838e0a452.png)


回答的质量得到显著的提升。
</details>

<details>
<summary> <strong>  有效提问5：通过真实的应用场景举例告诉我X的相关内容？</strong></summary>


以上4个有效提问是基于概念上的提问，接下来开始对作用上的提问。作用上的提问其实相当重要，有时候我会首先问这个问题。了解真实的应用场景，能够让你在学习该内容时将其与真实的应用场景联系起来，从而让你明白这个知识点的意义，也让你的学习会不那么枯燥。而且更重要的是，一般来说这里出现的应用场景就是你要在实践中去最后完成的任务。

![Pasted image 20230316205532](https://user-images.githubusercontent.com/69788237/227194113-8fa864a1-8536-4aa1-a484-8bd886a0ccf5.png)

继续深入了解的话可以选择其中一个应用场景，同时指定一种编程语言，让ChatGPT教你完成一段代码。比如：


![Pasted image 20230317020831](https://user-images.githubusercontent.com/69788237/227194265-96d7c4ef-7027-4221-86dc-9cf0fd35e6b0.png)
</details>

<details>
<summary> <strong> 有效提问6：请给我布置一些作业帮助我更好地理解和使用哈希搜索算法，布置的作业按顺序应该由浅到深，由简单到难</strong></summary>


<details>
<summary> <strong> 实践环节中的注意事项</strong></summary>

接下来进入实践阶段，你可以使用有效提问6来让ChatGPT给你布置一些作业，也可以通过在有效提问5中的深入来开始实践。我的推荐是使用有效提问6，因为一上来就做5中的实践可能过难。在进入这个阶段后，**与ChatGPT的交互就变得更重要，你要随时验证它的代码，并将自己的代码也汇报给它**。

首先可以确定一点，代码是一定要自己敲一敲的，但是为了效率，你并不需要从零敲起——实际上你要意识到，在有了ChatGPT后，任何代码都不再需要从零敲起。另外你也不需要一上来就敲出完整的、正确的代码。在最初，我们甚至可以不敲代码，只让ChatGPT进行演示，然后我们弄懂它给出的代码并进行反馈和交互直到代码完整且正确地运行即可。但到最后，你需要至少知道实现这个功能的整个过程，直到代码中每个变量和函数的作用才算过关。如果你觉得这个内容非常重要，就在完成以上步骤的情况下尝试完全自己自主完成这段代码，这会很有效地帮助你理解这个内容，但如果是不重要的内容，就可以留到后来要应用时再来复习。
</details>

![Pasted image 20230317021538](https://user-images.githubusercontent.com/69788237/227194376-4b5661fa-5064-4a7a-8477-86642f9d5d99.png)


接下来开始我们的第一个实践。先使用有效提问2和3了解作业中不了解的概念，比如作业1中的哈希表和Java中的HashMap。在了解所有的概念后，就开始进入写代码环节。在这个环节中，你可以选择让它只告诉你步骤（那么你要在提问中指明不需要给出具体的代码），自己来完成代码；也可以让它将整个代码给出，然后自己验证并学习一遍是如何操作的；这取决于这个知识点的重要程度，也取决于你的学习习惯。最低标准是，你至少能够看懂整个过程，能够以伪代码的形式将其复述出来。


![Pasted image 20230317024939](https://user-images.githubusercontent.com/69788237/227194442-5de0d51c-d689-4392-914c-f37566d6f6cb.png)


将以上代码复制进IDEA中运行并验证。

</details>

<details>
<summary> <strong>验证环节的注意事项</summary></strong>
验证环节实际上是非常重要的一个步骤，理论上来说我们应该对ChatGPT给出的每个回答都进行验证，但我们知道如果这样做，ChatGPT为我们节省的时间都被会用在验证上。如果验证出答案不正确还好，错误能够得到改正，花在这部分上的时间是有效的，反之则得不偿失。所以我们有必要弄清楚，什么是有必要验证的，以怎样的方式来验证。


以我的经验来看，对于一个初学者需要学习的内容而言，ChatGPT的正确率高得惊人。可以说只要你使用正确的提问方式，你基本可以认定ChatGPT的答案是正确的，而我们需要验证的主要是代码和复杂的、底层的概念解释。


#### 验证的方式

最简单的验证方式就是使用搜索引擎，将ChatGPT的回答直接复制到搜索引擎，看是否有相似的回答。这种验证方式简单快速，用于随时验证你觉得可能存在错误的回答。如果是一段代码，则将其复制进IDEA中看是否报错，运行结果是否达到你的预期。



</details>


<details>
<summary> <strong>Debug环节的注意事项</summary></strong>


不要只是简单地问“为什么”。ChatGPT给出的回答基于你所给出的反馈，如果只是问为什么，很可能因为缺乏相关背景而给出错误的回答。在这种情况下，你需要引导ChatGPT告诉你，你需要给出它怎样的信息才能够让它帮助你分析出真正错误的所在。


如果ChatGPT给出的代码出现错误，一般来说可以简单地归结为两种情况：（1）代码本身的错误 （2）代码不全，配置不全，代码前置条件不足的错误；两种不同的错误使用的提问不同。


对于第一种错误，首先自己要通读并理解代码，然后将报错信息、代码信息和你的需求一同复制给ChatGPT，并提出有效提问7，并询问如何修改才能达到你的需求。
</details>

<details>

<summary><strong>有效提问7：【给出报错信息】【给出全部代码或局部代码】，造成X的原因可能是什么，请分别罗列并告诉我哪个原因更可信，我应该如何提供给你什么信息才能使得你对原因做出更准确的分析？</summary></strong>

在Debug过程中，很少情况是能够一步到位的，往往需要多次反馈才能达到预期效果。如果我们只是问为什么会出现报错，我们得到的答案很可能是不准确或者不完全的，按照这个答案也可能会造成其它错误。这时候我们的提问不仅需要保证ChatGPT给出报错信息的解释，而且也给出进一步反馈所需要的信息。许多人在得到答案后不知道如何进一步与ChatGPT交互，实际上这一点也可以交给ChatGPT来告诉你。

![Pasted image 20230323195922](https://user-images.githubusercontent.com/69788237/227211629-5e16f708-4005-4529-90fa-9a1e2bdef303.png)



</details>

<details>
<summary><strong>有效提问8：在X之前，需要哪些准备工作？</summary></strong>
第二种错误会出现在你尝试使用ChatGPT开发较为复杂的功能时，这种错误更加隐蔽，因为代码本身可能没有任何错误，但是仍然无法运行或无法满足你的需求。

这些错误可能是因为你没有导入相关的依赖，这时候你要先使用有效提问8，问清楚ChatGPT代码是否完整，是否需要其它前置条件。

第二种错误实际上复杂得多，无法只是靠一两个问题就能迅速解决，这一点当你尝试开始开发项目时便会体验到，在下一篇文章我会尝试展开来讲如何解决这种错误。
第二种错误会出现在你尝试使用ChatGPT开发较为复杂的功能时，这种错误更加隐蔽，因为代码本身可能没有任何错误，但是仍然无法运行或无法满足你的需求。

这些错误可能是因为你没有导入相关的依赖，这时候你要先使用有效提问8，问清楚ChatGPT代码是否完整，是否需要其它前置条件。

第二种错误实际上复杂得多，无法只是靠一两个问题就能迅速解决，这一点当你尝试开始开发项目时便会体验到，在下一篇文章我会尝试展开来讲如何解决这种错误。


![Pasted image 20230316185135](https://user-images.githubusercontent.com/69788237/227199224-8d81464e-dbf2-447b-83e1-1f5fff0479de.png)


还有一种情况是因为版本更新一些功能不再能使用（比如在 2022年更新的Spring Security_ 5.7.0版本中 ，WebSecurityConfigurerAdapter这个class已经被弃用，而因为ChatGPT的信息是在2021年，它并不知道这个情况，所以仍会在代码中使用该class，结果导致代码错误）。这种情况就需要借用其它搜索引擎（此处推荐使用New Bing），比如搜索”WebSecurityConfigurerAdapter在最新版本中的Spring Security中是否还能使用“，你马上就会发现”WebSecurityConfigurerAdapter弃用“的搜索结果。

第二种错误对于初学者来说，如果没有事前意识到它们的存在，可能很难在实践中分辨出代码中究竟出现了什么错误，所以读者需要特别注意。
</details>

<details>
<summary><strong>如果ChatGPT无法解决你的问题</summary></strong>




首先尝试重新梳理自己的需求，将问题有条例地陈述出来，然后更换提问方式，从多个角度提问，补充更多条件，让ChatGPT更了解你想问的问题。

在确实经过多轮交互后仍无法解决问题时，在各大论坛或线下向更专业的人员咨询。

</details>

<details>
<summary><strong>学习完成后</summary></strong>



最后你能明白所有给出的代码且代码能够流畅运行，那么就算结束了。此外如果想进一步巩固，应该总结以上学习中的知识点和错误；最后自己再捋一遍全部代码，有必要的话也应该再完全自己写一遍代码，或者至少把思路（伪代码）写出来。

![Pasted image 20230318172030](https://user-images.githubusercontent.com/69788237/227194526-1f6144f4-ade6-4219-a1ae-ce4d73c27c92.png)

示例中的代码过于简单，所以没有任何错误，但在当你使用ChatGPT完成一段较为复杂的代码任务时，你会发现ChatGPT给出的代码会存在各种各样的细节错误，这很正常——这并不完全代表ChatGPT是“错误”的，这可能是因为你的沟通不到位，也可能是因为这部分细节应该由你来负责填补完成。

在这之后我们可以使用ChatGPT的Download插件，将整个页面下载下来作为笔记，以便未来随时参考。理论上来说，如果你的提问足够系统且完整，那么你甚至可以不再需要单独记录笔记。



</details>






## 最后

最后的最后，我希望读者理解很重要的一点是：借助合理的问题设计和背景补充，ChatGPT能够辅助你进行系统且有效地学习整个知识谱系，而不是只是应用于回答零散的知识点。想要使用好ChatGPT，将ChatGPT应用于你的学习，你有必要做好以下工作：

<ol>
<li>知道你所学习内容的知识谱系，或者说学习路径是怎样的。它应该包括你需要学习的所有内容，由浅到深排序——这一点你可以让ChatGPT帮忙。</li>
<li>捋清楚关于这些学习内容。是要学习关于它们的什么（是什么/为什么/如何做到），以怎样的方式来学习，这直接决定了我们应该如何设置我们的提问。</li>
<li>谨记ChatGPT的特性并把它应用于你的问题设计和交互中，在学习的过程中形成一套符合你的学科特性和你的学习方法、习惯的指令集。</li>
</ol>



这篇文章只是一个开始，接下来如果读者感兴趣的话，我将在下一篇文章中展示另外一种应用ChatGPT学习编程的方法——从各种意义上来说，这种方法都更实用，而且更符合编程学习的特性。我暂且称之为以项目为导向的学习方法（Project Orientied Method）。我将展示如何在ChatGPT的帮助下尝试开发一个较为复杂的Web应用程序项目，并在这个过程中，根据我们所遇见的困难学习我们所需要学习的内容。





   
    
    
 


<div align="center">
  <img src="https://user-images.githubusercontent.com/69788237/227213306-d3120e06-f1e9-46a8-875e-85608de6ad62.JPG" alt="Image 1" style="width: 150px; height: 160px;">
  <img src="https://user-images.githubusercontent.com/69788237/227213329-df40ed95-e9bf-4fc7-8763-d0979f69267a.JPG" alt="Image 2" style="width: 150px; height: 200px;">
   <br>
   <sub style="font-size: 12px; color: gray; max-width: 300px; display: inline-block; text-align: center;">我正在努力挣取我来年的留学费用中，如果以上的内容对读者有帮助，且您的手头尚有闲余，我会非常感激您的帮助。</sub>
   </br>
</div>



