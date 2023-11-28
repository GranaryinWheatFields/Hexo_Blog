---
title: Task orientation
date: 2023-10-31 15:23:46
categories:
- Easy to use
- Developing Quality Technical Information
---

# 任务导向

Task orientation.

## 为目标读者撰写

Write for the intended audience.

在你开始写之前，确保你对读者有一个清晰地认知。

例如，如果你的读者是管理人员，你可能只包含高层次的任务，如评估和规划，或其他任务的高层次概述。同样，如果你是为最终用户写作，请避免系统管理员的任务。

确保你在主题中包含的信息你的读者会感兴趣。例如，你的产品可能拥有一个强大的新帮助系统，但是对于正在安装产品的人来说，帮助系统功能的描述可能并不那么引人关注。

## 由用户视角呈现信息

Present information from the user's point of view.

从用户的角度撰写将用户融入“故事”中，使他们能够轻松地想象执行你所描述的任务。这样的写作具有以下特点：
- 主要以“你”（第二人称）为对象。
- 使用主动语态，使用表示用户执行的动作的动词，而不是产品执行的动作。
- 为这些动作提供原因。

> The system should not be shut down during processing. If such a shutdown occurs, the system should be restarted with the START RECOVER command.
>
> If you shut down the system during processing, you might lose data. Use the START RECOVER command to restart the system and recover any data from the log.
 

> Subsequent installation of the HIGS feature allows InfoProduct to run unattended.
>
> If you want to run InfoProduct unattended, you must install the HIGS feature. You can install the HIGS feature after you install InfoProduct.


## 确保提供信息时有切实可行的原因

Indicate a practical reason for information.

向用户提供所需信息只是任务导向写作的一部分。用户需要这些信息有一个实际的原因。他们需要了解你为何提供这些信息，以及它与他们的任务有何关系。信息所服务的目标必须是明显的。任务不仅仅是一种活动，而是朝着特定目标的活动。

为确保提供的信息与任务相关，请遵循以下准则：
- 在合适的情况下，将细节与任务关联起来。
- 在任务主题中仅提供必要的概念信息。

### 在合适的情境下，将细节与任务关联起来

Relate details to a task where appropriate.

在任务主题中，用户不应该产生疑问：“为什么要告诉我这个？” 例如，仅仅说明文件中的记录有一定的大小可能让用户感到困惑：“那又怎样呢？” 但是，如果你告诉他们他们必须构建一个用来保存文件的库，而记录的大小会影响到他们完成这项任务的方式，他们就能理解你为什么要告诉他们记录的大小。

> If the NORES option is used,the routines are link-edited as part of the load moudle.If the RES option is used ,the routines are loaded separately.
>
>  Use the NORES option when you have sufficient space for rountines to be link-edited as part of your load module.Use RES option to save space by loading the rountines only when you need them.

### 在任务主题中仅提供必要的概念信息

Provide only a necessary amount of conceptual information in task topics.

任务主题应着重提供仅支持任务的信息。任务主题可以包括：
- 完成任务的理由
- 完成任务的要求（如先决任务或软件）
- 任务的步骤
- 支持步骤的提示和示例
- 关于后续任务的信息（后置任务）

不要将大量重要的概念信息与任务信息混合。用户希望学会做事情，而无需学习与产品相关的所有概念。在任务主题中，尽早提供步骤，并且只在必要时简要解释次要概念。通过为每个主要概念创建一个单独的主题，将主要概念的解释与任务主题分开。在任务主题中提供到这些概念主题的链接。这样，已经理解概念的用户可以完成任务，而需要了解概念的用户可以转到概念主题。


> Creating test cases
> 
> You can create one or more test cases for each function that you want to test. 
> 
> Before you begin: 
> 1. Create a suite for the function that you are testing. 
> 2. Create a project within the suite to hold the test cases and files. 
>
> To create a test case: 
> 
> 1. Right-click a project and select New Test Case from the menu. 
> 2. Specify details in the New Test Case window. 
> 3. Click Record and work with the product that you want to test. 
> 4. Click Save after you finish recording your actions. 
> 
> Related topics
> 
> Creating suites、Creating projects、Suites、Projects、Test cases

## 专注于实际任务，而不是产品功能

Focus on real tasks, not product functions

实际任务是用户想要执行的任务，不论用户是否使用你的产品来完成。在技术写作中，你很容易忽略真正的任务，而陷入由产品决定的任务中。当使用一个产品几个月时，你可能会忘记用户的任务和产品的任务不一定是相同的。

用户想要编辑表格，但作者将这个任务表述为“使用表格编辑器”，而不是“编辑表格”。
用户想要统计文件中的记录，但作者将这个任务表述为“使用CNTREC实用工具”，而不是“使用CNTREC实用工具进行记录计数”。

有时产品的设计迫使你描述一些人为的任务。例如，用户想要创建图形，但必须首先设置一个容器来存放图形集。在这种情况下，你可以通过写作“使用容器组织图形”而不是“创建容器”来聚焦于任务而非设计。

## 使用显示任务的标题

Use headings that reveal the tasks

标题是向用户解释为何他们正在获取信息的首要地方。用户应从标题中获得关于主题内容的准确印象。每个标题都应明确表明主题包含与特定任务相关的信息，并概述该任务是什么。

一个像“授权”这样的静态标题对于概念或参考主题可能是可以的，但对于一个任务主题，标题应该揭示用户正在学习如何执行的任务。一个更有帮助的标题可能是“授权用户”或“为用户ID设置授权”。

## 将任务分解为离散的子任务

Divide tasks into discrete subtasks

在确定了主要任务之后，你需要将它们分解为离散的子任务，以便提供可用的步骤级信息。如果你尝试为撰写新闻报道这一主要任务提供步骤级信息，你可能会有成千上万个步骤。相反，你将写新闻报道的任务分解为其主要子任务，例如，研究材料，起草大纲，撰写初稿和修改草稿。重复分解任务的过程，直到你获得可以提供步骤级信息的任务组。

每个任务和子任务中的步骤数量应该是九个或更少。如果你发现一个任务需要超过九个步骤，要确定该任务是否可以再次分解，或者是否可以将一些步骤嵌套在其他步骤下。在编写任务信息之前，你需要了解任务与其他任务的关系。你需要了解任务的顺序、任务的级别和相互依赖关系。该任务是否真的是一个离散的任务？它是否有从属任务？它是更大任务的子任务吗？它是多个任务的子任务吗？

> Original
>
>    To migrate to version 8, you need to read these topics: 
>   
>       Hardware requirements
>   
>       Software requirements
>   
>       Applying the latest updates
>   
>       Stopping InfoProduct processes
>   
>       Backing up your infoproduct.inf file
>   
>       Running the migration utility for Windows
>   
>       Running the migration utility for UNIX
>   
>       Verifying migration
>   
>       Setting up a new profile

>    Revision 
>    To migrate to version 8: 
>    1. Ensure that you have the correct hardware and software: 
>    
>       Hardware requirements
>    
>       Software requirements
>    
>    2. Apply the latest updates. 
>    3. Stop all InfoProduct processes. 
>    4. Back up your infoproduct.inf file. 
>    5. Run the migration utility. 
>    
>       On Windows
>    
>       On UNIX
>    6. Verify the migration. 
>    7. Set up a new profile. 
>    After you finish migrating InfoProduct, you can start the processes again.

考虑这样一种情况，用户可能需要在安装之外的某个时候配置附加参数。对于用户来说，将验证安装的步骤与配置参数的步骤放在一起是没有意义的。此外，如果在 Linux 上验证安装的步骤与在 Windows 上的步骤相同，你可以将信息写一次，而不是在 Linux 主题和 Windows 主题中重复这些步骤。

确保将任务分解为离散的子任务，以确保每个子任务只包含一个明确定义的任务，但又包含足够的内容以独立存在。

## 提供清晰、逐步的说明

Provide clear, step-by-step instructions.

步骤构成了大多数任务。偶尔一个任务只有一个步骤，可以用一段文字描述，但大多数任务是按照有序的步骤执行的。任务导向延伸到最低步骤的级别。任何未清晰编写或顺序不正确的步骤都可能导致用户犯错或无法完成任务。

在编写任务信息时，通常你有机会及时发现可提出产品改进建议的可用性问题。例如，你可能会发现一些繁琐的步骤可以简化或避免，或者用户正在重复执行已经完成的操作（例如在多个窗口中输入长序列号）。如果在记录任务时遇到困难，请考虑产品工作方式是否存在问题。在写作过程中牢记用户的需求和兴趣；没有过于易用的产品这一说法。事实上，产品越易用，用户就越不需要依赖低级别的步骤信息。

花时间从用户的角度组织你的步骤。了解以下问题的答案：任务之间的关系是什么？步骤何时是子任务？什么构成一个步骤？步骤从何开始，何时结束？有些步骤是其他步骤的从属吗？哪些步骤是可选的？哪些步骤是有条件的？

以下几点指南可以帮助你提供清晰的逐步说明：

* 使每个步骤对用户来说都是明确的动作。
* 为了提高可用性，对步骤进行分组。
* 明确标识可选步骤。
* 在有条件的步骤之前明确标识标准。

### 使每个步骤对用户来说都是明确的动作

Make each step a clear action for users to take

每个步骤应该对应用户执行的一个动作（高层次或低层次的）。任务不讨论用户和产品如何交互；任务只列出用户完成任务时执行的动作。

确保每个步骤都明确描述了用户需要采取的具体行动，而不涉及用户和产品之间的交互细节。任务步骤应聚焦于用户的行为，使用户能够按照明确的指导完成任务。

> Original
>
> 1. Click OK. 
> 2. The installation begins. 
> 3. After installation completes, restart your system.
>
> Revision
>
> 1. Click OK. The installation begins. 
> 2. After installation completes, restart your system.

通过确保每个步骤都对应用户实际执行的动作，可以提高任务说明的清晰度和用户的操作准确性。

### 为了提高可用性，对步骤进行分组

Group steps for usability.

将步骤分组以帮助用户理解任务。如果按照一个接一个的顺序指导用户执行动作或点击，任务对用户来说可能会变得乏味。如果你能将次要步骤组合成一个更大的步骤，用户就可以将这些步骤与完成任务的目标联系起来。

例如，与其将步骤解释为“首先我在这里点击，然后填写那个字段，然后在那里点击，然后选择这个按钮”，用户可能更容易将步骤理解为“首先我设置我的偏好，然后我指定服务器信息”。通过这种方式，你不仅帮助用户理解他们正在执行的步骤，还简化了步骤，使每个步骤更容易被用户找到。

在编写任务说明时，考虑将相关的步骤组合在一起，形成更大的步骤，以促使用户更好地理解任务的整体流程。

> Original
> 
> To add a setting to your profile: 
> 1. Select the profile object that you want and right-click. 
> 2. Select Properties from the menu. 
> 3. In the Properties window, find the name and path of the profile file. 
> 4. Close the Properties window. 
> 5. Open your profile file in a text editor. 
> 6. Add the setting to your profile file in the settings section. 
> 7. Save the profile file. 
> 8. Run the profile command with the -file YourProfileName option.
> 
> Revision 
> 
> To add a setting to your profile: 
> 1. Determine the name of the profile file that you want to add the setting to: 
> 
>       a. Right-click the profile object that you want and select Properties from the menu. 
> 
>       b. In the Properties window, find the name and path of the profile file. 
> 
> 2. Update the profile file with the new setting: 
> 
>       a. Open your profile file in a text editor. 
> 
>       b. Add the setting to your profile file in the settings section. 
> 
>       c. Save the profile file. 
> 
> 3. Run the profile command with the -file YourProfileName option.

### 明确标识可选步骤

Clearly identify optional steps.

选步骤是用户可以跳过但仍然成功完成任务的步骤。在可选步骤支持任务的情况下，可以将其包含在任务中，并将其标识为可选。例如：“2. 可选：为启动参数定义配置文件。”

通过标识可选步骤，用户可以清楚地了解哪些步骤是对任务成功完成而言是非必需的，从而提高用户在执行任务时的自由度和选择权。

### 在有条件的步骤之前明确标识标准

Identify criteria at the beginning of conditional steps.

有条件的步骤是用户仅在符合某些条件时才执行的步骤。有条件的步骤通常以“如果”为开头，例如，“如果您以批处理模式运行测试用例，请在批处理页面上填写字段。” 符合步骤条件的用户必须按照这个步骤执行。始终从条件开始有条件的步骤。这样，不符合条件的用户在阅读条件后可以跳过这个步骤。

> Original
> 
> 1. Register your computer as a client if you are not yet registered on the LAN. 
> 2. In the Number field, specify your 12-digit serial number if your software is not yet registered. 
> 3. Run the InfoExec program to reconfigure your settings. (InfoExtended only)
> 
> Revision
> 1. If you are not yet registered on the LAN, register your computer as a client. 
> 2. If your software is not yet registered, in the Number field, specify your 12-digit serial number. 
> 3. InfoExtended only: Run the InfoExec program to reconfigure your settings.