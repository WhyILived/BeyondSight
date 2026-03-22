Looks better @: https://devpost.com/software/beyondsight-589mh7

🛠️ How we built it
From the moment we set foot in E7, we knew we wanted to tackle this challenge head-on. On Friday night, we secured an Xbox 360 depth camera off Facebook Marketplace, traveling across town on the 301 ION to pick it up. Meanwhile, our teammate Sy, a computer engineering student, brought a treasure trove of haptic motors to the table.

The hardware build began with 3D-printing the gauntlet to house the Braille keypad and motors, while wiring up the vest for navigation feedback. Simultaneously, we coded the AI communication pipeline—tying together:

Whisper for speech recognition
Gemini for natural language expansion
ElevenLabs for speech synthesis
Piece by piece, the hardware and software came together into a system where every component—from motors to models—worked in perfect harmony.

✨ What it does
BeyondSight is a fully wearable ecosystem designed to empower DeafBlind individuals with independence, communication, and safety.

👕 Navigation & Object Detection
Using an Xbox depth camera, the vest's four haptic motors guide the wearer through physical spaces. The motors on the left and right indicate turning directions, while the top and bottom motors guide vertical adjustments. With the gauntlet's Braille keypad, the user can request specific objects or destinations—whether that's a door, a chair, or even a water bottle. Once selected, the motors provide directional cues to help the user orient and reach the target.

✋ "Vibe Hand" & "Spidey Senses"
We designed unique interaction modes:

Vibe Hand uses rapid haptic pulses to deliver instructions for playful or cooperative actions, like playing catch.

Spidey Senses alerts the user when fast-approaching objects are detected, with all motors buzzing simultaneously to deliver an urgent warning.

🗣️ Conversational System
The gauntlet also acts as a two-way communication device:

User input via Braille is processed through the Gemini API, expanded into natural sentences, and spoken aloud with ElevenLabs through a portable speaker.

Incoming speech from others is captured with a microphone, transcribed via OpenAI's Whisper, then translated into Braille through six haptic motors on the gauntlet—allowing the wearer to "feel" the conversation in real time.

💻 Frontend & Backend Support
On the software side, we built a MongoDB-backed system to store user profiles, track conversations, and log locations. Genesys APIs enhance this by providing geolocation services and conversation summarization—offering caretakers or loved ones insights into where the user has been and what interactions took place.

💡 Inspiration
Our inspiration comes directly from someone close to us: our friend Damian—affectionately nicknamed Damy—who has been DeafBlind since childhood. Despite countless challenges, Damian made it all the way to the University of Chicago, showing resilience and determination that inspires us every day.

But we've also witnessed firsthand the struggles he faces: navigating unfamiliar spaces, trying to communicate in real-time, and depending heavily on others for basic independence. We wanted to build something that could transform those struggles into opportunities—not just for Damian, but for DeafBlind individuals around the world.

BeyondSight is our way of showing that accessibility isn't a luxury—it's a necessity, and with technology, it can become reality.

⚡ Challenges we ran into
Our biggest hurdle came from the Xbox camera itself. Because it's nearly two decades old, support is scarce. Our teammate Noah had to wrestle with:

Outdated drivers
Installing Ubuntu across multiple USB drives
Experimenting with Docker images
...before finally getting depth sensing and SLAM technology working.

Even once it ran, compatibility issues with Linux and the lack of modern documentation pushed us to the edge—but persistence paid off. In the end, we managed to breathe new life into a piece of legacy hardware and integrate it into a modern accessibility system.

🏆 Accomplishments that we're proud of
✅ Successfully configuring the old Xbox depth camera with Docker and Ubuntu to deliver real-time depth sensing.

✅ Designing and building a vest and gauntlet system that are both accessible and comfortable to wear, despite the complex wiring and motor placements.

✅ Optimizing OpenAI's Whisper pipeline, making it faster and more accurate in noisy environments than our initial tests.

✅ Creating unique haptic feedback modes like "Vibe Hand" and "Spidey Senses," which add both safety and fun to the experience.

📚 What we learned
"It ain't over 'til it's over." - Yogi Berra

This project taught us resilience more than anything else. Many of our hardware breakthroughs—like the camera setup and Whisper optimization—only came together in the final hours before presentations.

We learned to:

Stay calm under pressure
Keep experimenting when things looked impossible
Lean on each other's strengths
We also gained valuable hands-on experience with haptic hardware, multimodal AI systems, and accessibility design—skills we'll carry forward long after the hackathon.

🌍 The Current Market and What's Next
Accessibility technology is advancing rapidly, but solutions for DeafBlind individuals are still limited. Current tools often focus on one sense or one mode of interaction, leaving significant gaps. BeyondSight bridges those gaps by combining navigation, communication, and real-time safety into a single integrated system.

Studies show that people with disabilities consistently express a desire for greater independence and reduced reliance on caretakers. We believe BeyondSight is a step toward that reality.

🔮 Next steps include:
🎯 Replacing the bulky Xbox camera with lightweight, portable depth or LiDAR sensors.

🎯 Refining the haptic patterns through user testing with the DeafBlind community.

🎯 Optimizing for battery life and portability to make BeyondSight wearable for daily use.

🎯 Exploring partnerships with accessibility organizations to expand impact.

🌟 Our Vision
Our vision is bold but clear: make BeyondSight affordable, reliable, and available to DeafBlind people everywhere.
