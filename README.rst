line-bot-resources
==================

Introduction
------------
[Using rich menus](https://developers.line.biz/en/docs/messaging-api/using-rich-menus/)

Requirements
------------

-  Python >= 3.7

Getting started
---------------

::
    # 0. prerequisite
    $ export LINE_CHANNEL_ACCESS_TOKEN=YOUR_LINE_CHANNEL_ACCESS_TOKEN
    $ pip install -r requirements.txt

    # 1. upload all rich menus from `./rich_menu` directory using the filename as the alias_id
    $ python upload_rich_menu.py

    # 2. set rich menu to a user with the given `user_id``
    $ python set_rich_menu_to_user.py {rich_menu_id} {user_id}

    # set default rich menu to all users
    $ python set_default_rich_menu.py {rich_menu_id}

    # fetch all rich menus from LINE Platform
    $ python fetch_rich_menu.py

    # delete rich menu with the given rich menu id list (separated with spaces)
    $ python delete_rich_menu.py {rich_menu_id_1} {rich_menu_id_2} {rich_menu_id_3}
