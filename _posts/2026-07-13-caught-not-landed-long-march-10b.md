---
layout: post
title: "Caught, Not Landed: Why China's Booster Recovery Isn't a SpaceX Copy"
date: 2026-07-13
math: false
---

*On 10 July, China brought an orbital-class rocket booster home for the first time. It did not land it. It caught it, in a net, on a ship, using hooks instead of legs. The obvious reading is that Beijing has finally copied SpaceX. The engineering says something more interesting.*

The reflex, when China does something in space that the United States did first, is to reach for the word "copy." It is a comfortable reading and it usually contains some truth. It also fails badly here, and the way it fails is worth understanding, because the interesting question was never whether China could land a rocket. It was where you choose to put the mass, the precision, and the failure modes when you decide to bring a booster back.

There are only three known answers to that question, and on 10 July China demonstrated the third one.

## What actually happened

At 12:15 pm Beijing time on 10 July 2026 (0415 UTC), the first Long March 10B lifted off from the Hainan Commercial Space Launch Site at Wenchang. It is a two-stage vehicle, roughly 63 metres tall and 5 metres in diameter, with a liftoff mass around 760 tonnes and about 890 tonnes-force of thrust. Seven kerosene and liquid-oxygen engines power the first stage; a single liquid-oxygen and methane engine powers the second. In its reusable configuration it lifts about 16 tonnes to low Earth orbit, which places it in the same class as a Falcon 9.

The rocket put a satellite into its intended orbit. That satellite has not been publicly identified, and it is worth saying so plainly, because several write-ups name a specific payload that the primary reporting does not support.

The recovery is the story. About 150 seconds after liftoff, the stages separated at roughly 100 kilometres altitude. The first stage then flew a powered descent and, six minutes after separation, was captured on the deck of the *Linghangzhe* ("Navigator"), a purpose-built recovery vessel stationed more than 300 kilometres downrange in the South China Sea. It carried no landing legs. Instead, four hooks near the grid fins at the top of the stage engaged tensioned steel cables strung across the ship, and a hydraulic damping system absorbed what was left of the booster's energy. Auxiliary cables then locked the stage against wind and swell while a clamping platform moved in beneath it.

CASC called it China's first successful controlled recovery of a launch-vehicle first stage, and the world's first net-based recovery of any launch vehicle. Both claims stand up. The company says it intends to fly this same stage again before the end of 2026.

Two corrections to the coverage are worth making. First, this was not China's first attempt at the problem, but nor was it a case of third-time-lucky after two failures. In December 2025 the Long March 12A and Landspace's Zhuque-3 both reached orbit and both lost their boosters on the way down, but those are different vehicles built by different organisations. The direct precursor to this flight was in February 2026, when a Long March 10A test stage flew a maximum-dynamic-pressure abort test for the Mengzhou crew capsule and then, having done its primary job, performed a controlled propulsive descent to a splashdown deliberately placed beside the recovery vessel. February was the rehearsal. July was the catch.

Second, and this is the genuinely unusual part: nobody had previously recovered an orbital-class booster on a vehicle's maiden flight. Blue Origin tried on New Glenn's debut in January 2025 and lost the stage. SpaceX needed years of attempts. China succeeded on the first try, which is either very good engineering or very good luck, and probably some of both.

## Three ways to bring a booster home

Here is the part that repays attention. Every recovery architecture is a decision about where to spend mass and where to accept risk. There are three in existence, and they sit at genuinely different points in the same design space.

**Legs.** Falcon 9 and New Glenn carry their landing gear with them: legs, actuators, crush structure, reinforced hardpoints. All of it is dead weight on the way up, and every kilogram of it is a kilogram of payload you did not fly. The ground segment, by contrast, is dumb. A drone ship is essentially a barge with a flat top. The vehicle does all the work, which means the vehicle must be extremely precise: a legged booster has to arrive nearly vertical, nearly stationary, and inside a tight footprint, or it tips over.

**A tower.** Starship's Super Heavy carries no legs at all. It is caught near the top by mechanical arms on the launch tower. The mass moves off the vehicle and onto the ground, which is a real gain. But a tower is bolted to the launch site, so the booster has to fly home to it, and flying home means a boostback burn to cancel all that downrange velocity. Propellant spent flying back is propellant not spent lifting payload.

**A net on a ship.** The Long March 10B takes the tower's core idea, catching the stage near the top so it hangs in tension with no legs required, and puts it on something that floats. That is the clever bit. Because the catcher can move, it can be parked downrange along the booster's natural ballistic arc, so there is no expensive boostback burn. In principle this captures the tower's mass saving and the drone ship's propellant saving at the same time. CALT's own engineers make exactly this argument: no legs means lower dry mass and more payload, and a coordinated net widens the acceptable landing footprint.

That is not a copy of anything. It is a third answer.

## What it costs

Nothing in this trade is free, and the net's price is paid on the ground.

The *Linghangzhe* is not a barge. It is 144 metres long, 50 metres wide, displaces 25,000 tonnes fully loaded, and holds station using DP2 dynamic positioning. It is a substantial piece of capital engineering, and China currently has exactly one of them. A drone ship that gets damaged is an inconvenience. A recovery vessel that gets damaged, or is simply in the wrong ocean, is the whole capability.

The net is not passive either, which is the detail most of the coverage missed. According to CASC engineer Hao Jinjie, the cables sit on a movable mechanism that actively seeks out the descending rocket's hooks. CALT's Sun Zhenlian describes the whole event as a "two-way rendezvous": the booster steers toward the ship while the ship's cables move to meet the booster. Both ends of the problem are closing the loop simultaneously, on a deck that is itself pitching and rolling.

The obvious analogy is carrier arresting gear turned on its side, and Chinese engineers have reached for it themselves. It is a useful analogy for the energy-absorption function, hydraulic damping soaking up residual kinetic energy through a cable. It breaks down in one important place, and the break is worth naming: an aircraft that misses the wire is still flying and can bolter around for another attempt. A booster on final approach has no go-around. It gets one pass.

## The real achievement is the throttle, not the net

Now the mechanism that makes all of this possible, and which almost nobody is talking about.

A Falcon 9 booster cannot hover. Its single landing engine, even throttled to minimum, produces more thrust than the weight of the nearly empty stage, so its thrust-to-weight ratio never drops below one. The stage physically cannot hold station in the air. What it does instead is the hoverslam, sometimes called the suicide burn: it lights the engine at exactly the right instant so that its velocity and its altitude arrive at zero simultaneously. There is no margin in it. Burn early and you climb back up. Burn late and you cannot stop.

A hoverslam cannot be caught in a net. To be captured, a booster must arrive at essentially zero velocity relative to a ship that is moving in six degrees of freedom on the open sea, and stay there long enough for an active net to close on it. That requires the vehicle to be able to hover, or something very close to it. Which in turn requires an engine that can throttle down far enough for thrust to be balanced against the stage's weight rather than exceeding it.

This is precisely what the Chinese account describes. CALT designer Wang Cong breaks the return into four phases: coasting and attitude adjustment, powered deceleration, aerodynamic deceleration, and landing. Of the landing phase, the official technical description states that a "near-hover" control strategy is used, with grid fins and engines working together and an onboard trajectory planner generating the control sequence in flight. Three of the seven first-stage engines relight for the return burn; a single engine handles the final positioning.

Go back to February and it clicks into place. Among the technologies that flight explicitly validated on the descending core stage, alongside a high-altitude engine restart, was "hover ignition."

So the sequence reads: build an engine that throttles deep enough to hover, prove the hover on a test flight, then build a net you can only use if you can hover. The net is downstream of the engine. The genuinely hard thing China demonstrated on 10 July is not a piece of naval architecture. It is a propulsion system with a very large thrust turndown ratio and the guidance to exploit it, going from seven engines at liftoff to one deeply throttled engine holding a 5-metre-diameter cylinder nearly motionless above a moving ship.

Note the "near" in "near-hover," though. The stage does not arrive at a dead stop, which is exactly why the net needs hydraulic damping to absorb what remains. I have not seen published throttle ratios or terminal velocity figures, and I am not going to invent them.

## Why a commercial rocket matters to a lunar programme

The Long March 10B is not a standalone commercial vehicle. It is one member of a family, and it shares its 5-metre, seven-engine first stage with the crewed Long March 10A and with the core and boosters of the full Long March 10, the rocket intended to put Chinese astronauts on the Moon before 2030.

The full vehicle is a three-stage design whose core and two strap-on boosters are all the same module, which means 21 of these engines light at once. It stands about 90 metres, produces roughly 2,700 tonnes-force at liftoff, and is designed for 70 tonnes to low Earth orbit and at least 27 tonnes to trans-lunar injection. The lunar mission profile needs two launches: one Long March 10 lifts the Mengzhou crew spacecraft, another lifts the Lanyue lander, and the two meet in lunar orbit.

The consequence is that every commercial Long March 10B flight is also a flight test, paid for by a customer, of the exact propulsion module the crewed lunar rocket depends on. Ground testing cannot replicate real acoustic, thermal, and aerodynamic loading. This one can, and it builds a reliability record while doing it. That is a genuinely elegant piece of programme architecture and it deserves to be recognised as such.

It also deserves a caveat. Sharing a stage design is not the same as human-rating it, and the crewed variant has not yet flown to orbit. Its first orbital flight, carrying an uncrewed Mengzhou, is expected but has not happened.

## What we know, and what we don't

**Confirmed**, by CASC and CALT statements and corroborated across SpaceNews, Scientific American, Space.com, and Chinese state media: the launch date, time, and site; the maiden flight of the Long March 10B; insertion of a satellite into orbit; the recovery of the first stage by net capture on the *Linghangzhe* roughly six minutes after separation and more than 300 kilometres downrange; the vehicle's basic configuration and the vessel's dimensions; the four-phase descent with a near-hover landing phase; the February 2026 precursor flight; the December 2025 losses of the Long March 12A and Zhuque-3 boosters; and China's status as the second country, and CASC as the third organisation after SpaceX and Blue Origin, to recover an orbital-class booster.

**Not confirmed, and treated here as unknown:**

- **The payload.** Not publicly identified. Reports naming a specific satellite are not supported by the primary coverage.
- **The condition of the recovered stage.** This is the big one. "Complete success" is CASC's own characterisation. The orbital insertion can be independently verified by tracking the satellite. The health of the booster cannot be verified by anyone outside CASC, and a stage that is intact is not necessarily a stage that is flightworthy.
- **The refly.** Flying this stage again before the end of 2026 is a stated intention, not a demonstrated capability.
- **Refurbishment cost and turnaround time.** No data. Figures circulating online, including a 72-hour turnaround target, are unverified.
- **Throttle ratios, terminal velocity, and capture-window dimensions.** Sources conflict, including on the size of the net's opening. Insufficient data to resolve.
- **The black smoke.** Video of the descent shows heavy black smoke from the top of the stage during the powered phase. It has been widely observed and not, so far as I can find, publicly explained.

## The number that actually decides this

Three things here are real and should be said without hedging. China is the second country to bring an orbital-class booster home. It did so on a maiden flight, which no one else has managed. And it did so by a method nobody had used before, which represents a real and defensible point in the recovery trade space rather than an imitation of one.

And then the honest part. Recovery is not reuse. It is the entry ticket to reuse. On 9 July, the day before the catch, SpaceX flew a single Falcon 9 booster for the thirty-sixth time. Blue Origin recovered a New Glenn booster in November 2025 and flew it again in April 2026. CASC has recovered one stage, once, and has said it will fly it again. Until it does, and until somebody knows what the refurbishment actually costs, the economic argument for the net is a hypothesis. A booster you can catch but cannot cheaply refly is simply a very expensive net.

For an Indian reader the temptation is to file this under "China is ahead," and in launch cadence that is straightforwardly true. But it is the less useful reading. ISRO's Next Generation Launch Vehicle, Soorya, was approved by the Cabinet in September 2024 with a budget of ₹8,240 crore and a 96-month development window, and it is designed around a reusable first stage burning liquid oxygen and methane. The revealing detail is that VSSC is developing steerable grid fins and deployable landing legs, and ISRO issued a tender for landing-leg hardware in April 2026. India has already chosen its point in the same trade space, and it chose legs.

That choice is not obviously wrong, and 10 July does not make it wrong. It is a different answer to the same question: given your launch sites, your sea states, your industrial base, and above all your expected launch cadence, where should the mass live and where should the failure modes live? China's answer was to build a 25,000-tonne ship. That answer is entirely rational for a programme planning hundreds of constellation launches and a lunar landing, and it is not automatically the right answer for anyone else.

The booster came home. That much is real, and it is genuinely impressive. What it costs to send that same booster up again is the number that will decide whether any of it mattered.

---

*Sources: CASC and CALT statements as reported by Global Times, CGTN, and China Military; Andrew Jones for SpaceNews (10 July 2026); Scientific American, Space.com, Universe Today, and TechTimes coverage of the 10 July launch and recovery; Global Times reporting on the 11 February 2026 Long March 10A abort and descent test; Blue Origin and Space.com for the November 2025 New Glenn landing and its April 2026 reflight; Wikipedia and ISRO reporting for Long March 10 family and NGLV/Soorya programme details. Vehicle and vessel specifications are as stated by CASC and Chinese state media. The payload identity, the condition of the recovered stage, refurbishment economics, and the reflight timeline are not independently verified and are identified as such above.*
