    ..  important::
        When sent to the host via the :ref:`AddActivities` operation, the host is allowed and encouraged to replace this timestamp with the server's current timestamp.
        This allows the time-based ordering and filtering of :ref:`GetActivities` to be universally consistent and it avoids semantically-confusing requests from clients that have been disconnected for a while.
