---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
draft: true

description: "Description of the post (displayed in the post's card)"
categories: ["cat1", "cat2"]
displayInMenu: navigation menu (true, false)
displayInList: home page and category pages (true, false)

resources:
- name: featuredImage
  src: "/uploads/{{ title .Name}}.jpg"
  params:
    description: "{{ replace .Name "-" " " | title }}"
---