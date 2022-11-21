---
ms.openlocfilehash: 115103621cb0b156ebb7a3c2c72f0f303c497cfb
ms.sourcegitcommit: 47bd0e48c7dba1dde49baff60bc1eddc91ab10c5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/05/2022
ms.locfileid: "146178610"
---
{%- ifversion restrict-groups-to-workflows %}
1. Назначьте политику доступа для рабочих процессов.

   Группу средств выполнения можно сделать доступной для определенного списка рабочих процессов или для всех рабочих процессов. Этот параметр нельзя переопределить, если вы настраиваете группу средств выполнения в организации, которая используется совместно в предприятии. Указывая, какой рабочий процесс может получить доступ к группе средств выполнения, необходимо использовать полный путь к рабочему процессу, включая имя и владельца репозитория, а также нужно прикрепить рабочий процесс к ветви, тегу или полному значению SHA. Например: `octo-org/octo-repo/.github/workflows/build.yml@v2, octo-org/octo-repo/.github/workflows/deploy.yml@d6dc6c96df4f32fa27b039f2084f576ed2c5c2a5, monalisa/octo-test/.github/workflows/test.yml@main`. 
   
   Доступ к этой группе средств выполнения будут иметь только задания, непосредственно определенные в выбранных рабочих процессах.{%- endif %}