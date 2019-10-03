---

    @snap[north span-100]
    #### Fenced Code Block
    @snapend

    ```
    defmodule GenMetrics.GenStage.Monitor do
        use GenServer

        alias GenMetrics.GenStage.Manager
        alias GenMetrics.GenStage.Monitor
        alias GenMetrics.GenStage.Pipeline
        alias GenMetrics.GenStage.Window
        alias GenMetrics.Reporter
        alias GenMetrics.Utils.Runtime

        @moduledoc false
        @handle_demand :handle_demand
        @handle_events :handle_events
        @handle_call   :handle_call
        @handle_cast   :handle_cast

        defstruct pipeline: %Pipeline{}, metrics: nil, start: 0, duration: 0
    ```
