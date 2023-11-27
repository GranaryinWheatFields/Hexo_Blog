---
title: Easy to use
date: 2023-10-31 15:23:46
categories:
- 文档写作理论
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


# 准确性

Accuracy.


# 完整性 

Completeness.