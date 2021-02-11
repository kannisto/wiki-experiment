
# Wiki experiment

This is how code can be inserted:

    {
        // *** Messages MUST be encoded in UTF-8! ***

        // --- Fields of AbstractMessage begin ---
        "Type" : "set-message-type-here",
        "Timestamp" : "2020-06-03T04:04:21.045Z",
        "SimulationId" : "2020-06-03T04:01:52.345Z",
        "SourceProcessId" : "set-process-id-here",
        "MessageId" : "set-message-id-here",
        // --- Fields of AbstractMessage end ---

        "SimulationState" : "running",
        "Name" : "Name of the simulation",
        "Description" : "Longer description about the simulation"
    }

This thing supports even tables:

| Field | Type | Multiplicity | Explanation |
| ---- | ---- | ---- | ---- |
| All fields from [AbstractMessage](subsub1.md) |  |  | Fields from the "abstract base class" |
| SimulationState | String | 1 (REQUIRED) | Simulation state, either: "running" or "stopped" |
| Name | String | 0..1 (OPTIONAL) | A human friendly name for the simulation. |
| Description | String | 0..1 (OPTIONAL) | A longer description of the simulation run meant for humans. |
