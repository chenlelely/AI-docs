# GPT2介绍

#### 基本情况

官方介绍：https://blog.openai.com/better-language-models/

论文：https://d4mucfpksywv.cloudfront.net/better-language-models/language-models.pdf

代码：https://github.com/openai/gpt-2（只有使用GPT2的代码，**模型训练代码没有公布**，据说不会公布）

预训练模型：只有较小的一个117M模型，**完整的模型没有公布**（据说再考虑６个月决定是否公布）

性能：官方宣称不针对具体任务做训练，在多个测评中就能超过已有的所有模型，甚至接近人类水平

语言：经实验，目前**只有英语，而且不会有中文模型发布**。官方回应可以输出中文，但不知如何做到；所有的训练素材都是英语。

亮点：**能够生成流畅的文本，接近人类的水平**。

缺点：

- 针对专业领域，生成的质量可能较差（可能跟训练语料有关）。

  > on highly technical or esoteric types of content, the model can perform poorly.

- 可能会有重复(repetitive text)、world modeling failures、主题不连贯(unnatural topic switching)等问题

  > we have observed various failure modes, such as repetitive text, world modeling failures (e.g. the model sometimes writes about *fires happening under water*), and unnatural topic switching. 


#### 结论

1. 看起来很好

2. 无法直接应用在项目中，面临着以下困难：

   - 不支持中文
   - 没有训练代码，无法自己训练模型
   - 没有公布完整的模型

3. 可以考虑根据他们的论文，自己实现模型然后进行训练？（论文中没有详细介绍模型，只模糊的提到是基于Transformer架构的LMs，跟GPT模型大致类似，做了一些改动。）


生成示例：

> There are several locations in North Carolina (and beyond) where Larry has chosen to publish and write. In contrast to many of these places, this North Carolina is not one where Nevada and Colorado have become centralized. The situation with Grandma, in particular, is quite different.
>
> A Box comes out in February 2018. But you are on Android and Windows, and could ban your Nintendo-cast gaming device (and download AC 4.2). Buy cartridges from your Arcade Partner with MLB.TV or provide copies through joint Starbox.com.
>
> A Starter Clock may be coming out over okay cold Bellingham, SEA at 7 a.m.. World Hack Store Nov. 25, 2018 PT: Ticket-box's PlayStation Channel broadcasts official Pokemon Championship tournament results.
>
> If you heard some couple of weeks from him, I didn't hear any names of a specific hunch he was untruthful or is being manipulated to oppose what he says.









