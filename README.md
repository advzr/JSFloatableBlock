JSFloatableBlock
================

A javascript plugin to create floatable blocks

Depends on jQuery.

Features:
- does not require any specialy ordered blocks in DOM
- can handle unlimited queues of floatable blocks
- a queue can be interupted by a bumper block with css class of 'fb-bumper'

How to use
- all blocks should be positioned absolutely.
- the plugin searches for blocks with css classes beginning with 'floatable-block-' and creates queues of blocks with equal classes (that is the plugin will find blocks with classes like 'floatable-block-abc' and 'floatable-block-def' but will create 2 queues because there are 2 different classes in DOM).
- blocks stop when they reach a block with 'fb-bumper' class.
- by default a block starts floating when the distance between the browser window and the block equals 0px. But this can be overridden by adding 'data-margin-top' attribute.
- by default a block stops when it reaches either an another floatable block or a bumper when the distance between them equals 'data-margin-top' (if set) or 0px (if data-margin-top is not set). But this can be overridden by adding 'data-margin-bottom' attribute.
