# What could have been better?

When trying to improve performance, it is best to narrow down what exactly is causing it not to be so performant. In my case I should've used React Profiler and also thought of each state update. The rendering of the create delivery dialog wasn't actually expensive, but it was loading and rendering all the datasets that made it expensive.

# Did you do anything outstanding?

I think it was great that I looked up Kent's resources for react performance, as I found virtualization there, it made me realise that the Data Grid itself should virtualize the grid. In our case it was disabled due to SSR reasons, but it should be enabled on the client.

# What did you learn?

I did learn working with React profiler and checking the time for each render of each component, it was actually way easier than I thought working with it and profiling.

# Overall what are your feelings and are you happy with how the workday went?

I'm really happy how the day went, felt like I got a lot of things done and I didn't ignore the slowness of the Data Grid, but instead took action as a software craftsman should do, and care for the quality and understand that it isn't a good experience for our customers.

I also realised that we might need XState in the near future, especially on the share id page where we have so many buttons, transitions, deliveries and now automations being made.

I think it will require some architecture and mob thinking around it though.
