---
layout: post
title: "Eye in the Sky: The Netra AEW&C and Its Long Road to Combat-Ready"
date: 2026-06-29
math: false
---

*On 25 June 2026, India declared its indigenous Netra airborne early-warning system fully combat-ready. The certificate was dedicated to eight people who died chasing the same idea twenty-seven years earlier. This is the engineering story in between.*

On 11 January 1999, a modified Avro HS-748 turboprop took off from Arakkonam in Tamil Nadu carrying an experimental radar dome and a crew of scientists and air force officers. It never landed. The crash killed all eight on board, four DRDO scientists and four IAF personnel, and it effectively ended India's first serious attempt to build an airborne early-warning aircraft.

Twenty-seven years later, on 25 June 2026, the program that rose from that wreckage reached the finish line. At the Centre for Airborne Systems in Bengaluru, the Indian Air Force received Final Operational Clearance for the Netra AEW&C system, certifying it as fully combat-ready. The clearance was dedicated to the crew lost in 1999.

That arc, from a crash site to a cleared combat system, is worth understanding in detail, because the hard part was never the idea. Everyone wants an eye in the sky. The hard part is the engineering: bolting a high-power radar onto an aircraft that was never designed to carry one, keeping it cool, keeping it stable, and turning what it sees into something a fighter pilot can use in time.

## What "final clearance" actually certifies

A modern AEW&C platform is what engineers call a system of systems: a radar, an electronic-warfare suite, communications, mission software, and the airframe itself, all of which have to work together under stress. Final Operational Clearance is the certificate that says all of it does, across the full envelope of conditions the air force expects to fight in. It comes after Initial Operational Clearance, which Netra reached around 2017, and after years of trials, refinement, and real operational use.

The cleared fleet is small: three Netra Mk1 aircraft, flown by No. 200 Squadron from Bhisiana Air Force Station near Bathinda, Punjab. The significance is larger than the number. With FOC, India joins a short list of countries that can design, integrate, and field an AEW&C suite of this complexity on their own rather than buying one. Roughly three-quarters of Netra's mission electronics are indigenous.

## The problem with putting a radar on a regional jet

Netra is built on the Embraer ERJ-145, a Brazilian regional jet chosen for reliability and running costs. It was emphatically not designed to carry a radar array on its back. Doing so created three distinct engineering problems, and all three had to be solved at the same time.

The first is aerodynamic. The radar lives in a dorsal structure called the Active Antenna Array Unit, an elongated plank roughly eight metres long, mounted on four reinforced pylons above the fuselage. Hanging a structure like that on top of an airframe shifts its centre of gravity and moves the point where aerodynamic forces act. Worse, the array sheds a turbulent wake that streams back toward the vertical tail, the surface the aircraft depends on for directional stability and control. Engineers at DRDO and the National Aerospace Laboratories worked through this with extensive CFD analysis and wind-tunnel testing, modifying the empennage and rewriting flight-control laws so the aircraft stays controllable across its full range of pitch and yaw, including the asymmetric cases that matter most. The first flight of a modified airframe, in 2011, was flown with a dummy mass simulator standing in for the real array, purely to prove the aircraft could handle the change before any electronics went aboard.

The second problem is heat. An active array is thousands of small transmit-receive modules, and at full power they dump tens of kilowatts of waste heat into a confined structure. Let the modules run too hot and their performance drifts or they fail outright. The cooling design had to guarantee airflow to every module even when the air around the array is disturbed by the aircraft's attitude or by the nearby satellite-communications radome.

The third is power. The radar, the mission computers, and the environmental control system together draw far more electrical power than a regional jet normally generates, so the aircraft was fitted with uprated generators and a dedicated auxiliary power unit for the mission systems. An in-flight refuelling probe was added as well, stretching endurance from roughly five or six hours to around nine. That is the difference between a short look and a persistent watch over a contested border.

## A radar with no moving parts

The heart of Netra is its radar, developed by the Electronics and Radar Development Establishment. Older airborne radars spin a dish to sweep the sky. Netra's array is fixed and steers its beam electronically, which lets it look in different directions almost instantly and run search, tracking, and target prioritisation concurrently rather than one after another.

The array reflects a neat piece of indigenous packaging. Eight individual transmit-receive modules are fused into a single unit to save space inside the slim plank, and these units are tiled across two flat faces mounted back to back. Reported figures put it at roughly 2,560 modules in total, operating in the S-band and built on gallium-arsenide semiconductors. The two faces give the radar a 240-degree field of view, 120 degrees out to each side.

That number, 240 degrees, is also Netra's central limitation, and it explains a great deal of what comes after. Two faces looking sideways leave a wedge of about 60 degrees uncovered off the nose and another off the tail. When the aircraft flies the long racetrack orbits that keep it on station, those blind cones sweep through the sky, leaving gaps that have to be filled by ground radar or a second aircraft. It is the price of fitting a fixed array onto an airframe this size.

Within its coverage, the radar is credited with detecting fighter-sized targets at around 250 to 375 kilometres, with longer instrumented tracking ranges reported under good conditions. One of the quieter wins between IOC and FOC was in software, not hardware: refining the Doppler processing that picks genuine low-flying targets, cruise missiles and drones skimming the terrain, out of the enormous clutter of the ground behind them. That capability is where AEW&C earns its keep, and it ties directly to a problem worth spelling out later.

| Netra Mk1 — key parameters | |
|---|---|
| Platform | Embraer ERJ-145 (EMB-145I) |
| Radar | Indigenous AESA (LRDE), S-band, gallium-arsenide |
| Coverage | ~240° azimuth (120° per face; ~60° blind cones fore and aft) |
| Detection (fighter-sized) | ~250–375 km (reported) |
| Fleet / unit | 3 aircraft, No. 200 Squadron, Bhisiana AFS |
| Endurance | ~9 hours with in-flight refuelling |
| Indigenous content | ~75% of mission suite |
| IOC → FOC | ~2017 → 25 June 2026 |

*The detailed radar figures above are as reported in open sources; DRDO has not officially disclosed precise numbers.*

## Seeing without being seen, and sharing what you see

A radar that broadcasts is also a beacon, so Netra carries a parallel set of passive sensors. Its electronic-support and communication-support suites listen across the spectrum, locating and fingerprinting hostile radars and intercepting communications without emitting anything detectable. Because an AEW&C aircraft is itself a prime target, it also carries a self-protection suite: warning receivers, a missile-approach warning system that uses infrared sensors to catch the heat bloom of a launch, and dispensers that throw out chaff and flares to defeat radar- and heat-guided missiles.

The sensors are only half the system, though. The real product of an AEW&C aircraft is a single fused picture of the air situation, stitched together from radar, passive sensors, and datalinks, then shared across the force. Netra can network with a reported forty-odd assets at once, and it can vector friendly fighters onto a target without those fighters switching on their own radars, which would give away their position. The same picture is pushed down to transportable ground stations that feed the air force's wider command-and-control network. Early in the program the original radios were replaced with software-defined radios to keep pace with modern encrypted links. A fighter that stays radar-silent and still arrives in a firing position with full situational awareness is the entire point of the exercise.

## What combat has, and hasn't, shown

Netra has flown in anger. During the Balakot airstrikes in February 2019 it provided surveillance and early warning, helping deconflict airspace and watch for the Pakistani response. During Operation Sindoor in May 2025, the four-day India-Pakistan clash that followed the Pahalgam terror attack, AEW&C aircraft were part of the networked air battle; by several accounts the platform that flew operationally was actually the Netra Mk1A development testbed.

A note of caution is in order here, and it matters for anyone trying to draw the right lessons. Much of the dramatic reporting around Sindoor, including a widely circulated claim that an Indian S-400 battery downed a Pakistani Saab 2000 Erieye early-warning aircraft at a record 314 kilometres, originates with Indian sources and was reportedly affirmed afterward by the IAF chief. Pakistan disputes it, and independent verification has not emerged. Both sides took losses, and the precise tally remains contested. I am not going to repeat any specific kill count as established fact, because at this point it isn't one.

What is worth taking from Sindoor is the underlying principle, which holds regardless of the box score. A ground-based radar cannot see a low-flying target far past the horizon; the Earth curves away, and an aircraft or cruise missile down low drops out of view within a few tens of kilometres. A platform orbiting at altitude sees much farther, and when its track is handed by datalink to a long-range surface-to-air missile, that missile can be guided through the middle of its flight toward a target the launcher itself may not hold cleanly. An elevated sensor plus a long-range effector, tied together by a network, is what lets a modern air defence reach well beyond any single radar's coverage. Netra is built to be one of those elevated sensors, and that role does not depend on any particular contested headline being true.

## Mk1A, Mk2, and closing the gap

The Mk1 fleet's limitations double as the roadmap for what comes next. The government has approved six more aircraft in the Netra Mk1A configuration, which keeps the proven Embraer airframe but moves the radar to gallium-nitride modules. GaN handles heat and power more efficiently than gallium-arsenide, which translates into more transmit power and better range from a similar array. Beyond that sits the larger Netra Mk2, planned for a bigger aircraft with more electrical power, more operator stations, longer endurance, detection ranges past 500 kilometres, and the wider coverage that finally closes the Mk1's blind cones.

The trajectory is the real story. A three-aircraft fleet certified today is the foundation for a genuine airborne-surveillance ecosystem meant to watch two long and very different borders at once.

## The part worth remembering

Final Operational Clearance is not a dramatic moment. There is no fireball, no launch, no record to announce. It is a certificate that says a hard problem has been solved properly, that the thing works across the conditions that count, reliably enough to be trusted with lives. Behind that certificate sit more than two decades of aerodynamics, thermal engineering, radar physics, software, and systems integration, carried out by people who took over a program that had already cost eight lives and saw it through to the end.

That is the part worth holding on to the next time a headline reaches for the word "breakthrough." The eye in the sky was not a breakthrough. It was a long, patient, unglamorous climb, and on 25 June it finally reached the top.

---

*Sources: Ministry of Defence release and PTI reporting (via The Week), Air Force Technology, Business Today, and India Sentinels coverage of the 25 June 2026 FOC ceremony; standard accounts of the 1999 ASP crash and the October 2004 Cabinet Committee on Security re-sanction; DRDO/CABS programme descriptions. The Operation Sindoor engagement claims referenced here are reported by Indian sources and disputed by Pakistan, with no independent verification to date; they are presented as contested rather than confirmed. Several detailed Netra specifications are as reported in open sources and have not been officially disclosed by DRDO.*
