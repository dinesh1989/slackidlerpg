1. Extract out the redis logic.
  - I shouldn't have to care about single vs. multi

2. Multi-slack support
  - Need to store token when oauth'd

3. Calculate penalty for going away/returning, and parting/joining
  - can't subscribe for that as event without RTM, which is annoying
  - have to check whether user's status has changed since we last checked
  - (I think we can subscribe to user parts/joins)

3. Calculate penalty for other actions - starring, starting a thread in channel, etc.

4. How is idlerpg going to know which channel it should live in?
  - might be easiest to just hardcode it for now

5. Should @mention users during announcements

6. Better display for "time to level", instead of just a number of seconds.