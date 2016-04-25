# Azure Webjobs SDK Processors for Azure ServiceBus Pipelines

## Introduction
This assembly will enable different processors to be used in a [pipline][3].

Built-in pipelines

1. `HalfLifeRenewMessageProcessor`: automaticaly renew the message every halflife

## Our use case
We have 2 [WebJobs Extensions][1], one to implement [pipelines][3] for the [ServiceBus][2] subscription [trigger][5] and one for a Topic Level [trigger][4])
We didn't want to duplicate the code so this assembly was made.

## Installation
You can obtain it [through Nuget][0] with:

    Install-Package Pandora.Azure.WebJobs.PipelineCore.Processors

Or **clone** this repo and reference it.

[\\]: Refrences
[0]: https://www.nuget.org/packages/Pandora.Azure.WebJobs.PipelineCore.Processors
[1]: https://github.com/Azure/azure-webjobs-sdk-extensions
[2]: https://azure.microsoft.com/en-us/documentation/services/service-bus
[3]: https://github.com/PandoraJewelry/WebJobs.PipelineCore
[4]: https://github.com/PandoraJewelry/WebJobs.Extensions.TopicTrigger
[5]: https://github.com/PandoraJewelry/WebJobs.Extensions.ServiceBusPipeline
