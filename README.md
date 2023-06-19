Reimplementation of API used in hector.network for governance purposes.
This app was born because the team arbitrarily removed voting power from multiple fNFT holders without mandate of the DAO. Community requires properly working API to facilitate voting without teams censorship. Webapp offers two endpoints serving two versions of API. Community is free to use the one they deem "right".


#### /voting-power
Each fNFT has voting power equal to the amount of HEC that was used to mint it.

If you lock 10 HEC you get 10 voting power. 

If you locked LP containing 10 HEC and 40 USDC you get 10 voting power.

To my understanding of (currently deleted) project documentation this is what was intended since project launch and is in +95% of cases (not counting burnt fNFTs) equal to what the original API used to serve. 
Differences exist in a bunch of fNFTS minted between 2022-11-02 and 2022-11-10 that have increased voting power by few % (up to 7%). 
I'm not aware of why that is and I couldn't find anything about any governance power boosts in (deleted) project documentation. Asking the current team is also impossible because they banned me from the project's discord server for asking too many questions ;)

#### /voting-power-with-boosts
This version tries to be as close as possible to what the original API used to be. 

All voting powers except those that the team changed to zeros are copied from the original API. 
Those zeroed are rebuilt using same approach as explained above in /voting-power


API is currently hosted at http://asfweasdf.pythonanywhere.com/voting-power

Built with :heart: for DAOs.


_“We must learn that passively to accept an unjust system is to cooperate with that system, and thereby to become a participant in its evil.”
― Martin Luther King Jr._
