.. _person type:

Person
~~~~~~

A person has the following properties.

..  include:: /_fragments/person_provider_id.rst

Name
    A **string** of the user's friendly name. Optional.

PictureUrl
    A **string** with a url to a profile picture of the user. Optional.

    ..  note::
        This property is only expected to be returned by the server.  Clients do not need to populate it when making a request to the server in an operation like :ref:`AddActivities`.

Relationships
-------------
Each person has several optional properties that may be set to describe the person's relationship to the activity.  As usual, all properties default to false and should not be included when they are false.

Mentioned
    A **boolean** property indicating this person was explicitly mentioned in the activity, for example via a mention activity.

InThread
    A **boolean** property that indicates that this user was part of a threaded discussion but was not explicitly involved in this activity.  For example, a threaded comment discussion.

RepliedTo
    A **boolean** property that indicates that this user is the parent of a piece of content that this activity is replying to.  For example, a reply in a threaded comment discussion.

Creator
    A **boolean** property that indicates that this user is the person who created the activity.  This is omitted on AddActivities calls; the host should determine the creator via the access token used on the AddActivities request.
