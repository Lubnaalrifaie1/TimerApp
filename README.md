# TimerApp
## **TimerApp: A Rust Command-Line Timer**

# **Description:**
TimerApp is a lightweight and easy-to-use command-line timer application written in Rust. It allows users to track the elapsed time between starting and stopping a timer. The primary focus is on simplicity and providing a straightforward interface for time tracking.

# **Features:**

1. **Command-Line Interface:**
   - TimerApp is designed to be used through the command line, making it convenient for quick time tracking without the need for a graphical user interface.

2. **Timer Functionality:**
   - Users can start and stop timers using command-line arguments.
   - Timers are identified by a name, which can be specified by the user or defaults to "local."

3. **Multiple Timers:**
   - TimerApp supports the creation of multiple timers simultaneously, each with its own unique name.
   - Timers are stored in a HashMap for easy retrieval and management.

4. **Time Display:**
   - The application provides feedback on the elapsed time of a timer when queried.
   - The time is displayed in a duration format, showing the hours, minutes, and seconds.

5. **Chrono and Clap Integration:**
   - The project leverages the `chrono` crate for date and time handling and the `clap` crate for parsing command-line arguments.

6. **Error Handling:**
   - While basic error handling is in place, users are informed through the command line in case of conflicts or other issues.

7. **Extendable:**
   - The code is structured to allow for easy extension and modification, making it a good starting point for additional features or customization.

# **Usage:**
- To start a timer: `TimerApp timer --start [--name <timer_name>]`
- To stop a timer: `TimerApp timer --stop [--name <timer_name>]`
- To check the elapsed time of a timer: `TimerApp timer --name <timer_name>`

# **Example:**
```bash
$ TimerApp timer --start --name work
Timer 'work' started.

$ TimerApp timer --stop --name work
Timer 'work' stopped.

$ TimerApp timer --name work
Timer 'work': 1h 30m 15s
```

**Note:** The provided code is a foundation for a timer application, and additional features or improvements can be implemented based on specific use cases or user requirements.
