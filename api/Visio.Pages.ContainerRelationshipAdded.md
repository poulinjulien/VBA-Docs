---
title: Pages.ContainerRelationshipAdded Event (Visio)
keywords: vis_sdr.chm11062065
f1_keywords:
- vis_sdr.chm11062065
ms.prod: visio
api_name:
- Visio.Pages.ContainerRelationshipAdded
ms.assetid: 8d7480e7-0131-8c02-11ad-d5784679e387
ms.date: 06/08/2017
---


# Pages.ContainerRelationshipAdded Event (Visio)

Occurs when a new container relationship is added to the document.


## Syntax

Private Sub  _expression_ _'ContainerRelationshipAdded'(**_By Val ShapePair As RelatedShapePairEvent_**)

 _expression_ A variable that represents a '[Pages](Visio.Pages.md)' object.


### Parameters



|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
| _ShapePair_|Required| **[RelatedShapePairEvent](Visio.RelatedShapePairEvent.md)**|An object that represents the new container shape-pair relationship.|

## Remarks

The  **RelatedShapePairEvent** object that this event returns contains two shapes: the container and the member, represented by the **[RelatedShapePairEvent.FromShapeID](Visio.RelatedShapePairEvent.FromShapeID.md)** and the **[RelatedShapePairEvent.ToShapeID](Visio.RelatedShapePairEvent.ToShapeID.md)** properties respectively.

If you are using Microsoft Visual Basic or Visual Basic for Applications (VBA), the syntax in this topic describes a common, efficient way to handle events.

If you want to create your own  **[Event](Visio.Event.md)** objects, use the **[EventList.Add](Visio.EventList.Add.md)** or **[EventList.AddAdvise](Visio.EventList.AddAdvise.md)** method. To create an **Event** object that runs an add-on, use the **EventList.Add** method. To create an **Event** object that receives notification, use the **EventList.AddAdvise** method. To find an event code for the event you want to create, see [Event Codes](../visio/Concepts/event-codesvisio.md).


