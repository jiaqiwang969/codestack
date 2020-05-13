---
layout: article
title: Write custom properties to all sources using Document Manager API
caption: Write All Properties
description: VBA macro to write custom properties to all sources (file, configuration, cut-list items) using Document Manager API
lang: en
image: /solidworks-document-manager-api/document/data-storage/custom-properties/write-all-properties/added-custom-property.png
labels: [write properties]
---
{% include img.html src="added-custom-property.png" width=450 alt="Custom property added to the file" align="center" %}

This VBA example demonstrates how to add the *ApprovedBy* property with the value of the name of current user to all sources using Document Manager API. Property will be added (or updated) for the file (general), all configurations and all cut-list items.

Specify the full path of the file in the *FILE_PATH* constant.

{% include_relative Macro.vba.codesnippet %}