Mention Activity
----------------

A mention activity indicates that the user has mentioned another user, perhaps via an @user syntax.  Mention has the following key/value pairs in its Data object:

ParentContentId
    A **string** identifying the ContentId of the part of the document that contains this mention. For example, if this mention takes place inside a comment, then this mention's ParentContentId is the ContentId of that comment. Maximum length 1024 unicode characters. Optional.

..  include:: /_fragments/activities/common_content_data.rst

A mention activity should have one :ref:`person <person type>` in its People array who represents the person who was being mentioned.  That person must have Mentioned=true set.