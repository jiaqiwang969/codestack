---
layout: article
title: Handling dynamic values updated in the controls
caption: Dynamic Values
description: Handling dynamic values updated in the controls of the Property Manager Page using SwEx.PMPage framework
lang: en
image: /labs/solidworks/swex/pmpage/controls/dynamic-values/controls-dynamic-values.gif
toc_group_name: labs-solidworks-swex
order: 13
---
{% include img.html src="controls-dynamic-values.gif" alt="Values updated controls" align="center" %}

In order to update control values for the properties changed from the code behind dynamically (e.g. on button click or when one property is changing another property), it is required to implement the [INotifyPropertyChanged](https://docs.microsoft.com/en-us/dotnet/api/system.componentmodel.inotifypropertychanged?view=netframework-4.8) in the data model. Raise the [PropertyChanged](https://docs.microsoft.com/en-us/dotnet/api/system.componentmodel.inotifypropertychanged.propertychanged?view=netframework-4.8) event for every property which needs to be watched to notify the environment that value has changed and control needs to be updated.

{% include code-tabs.html src="DynamicValues" %}