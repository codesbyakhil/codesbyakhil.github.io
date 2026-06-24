---
layout: post
title: "Slow on Purpose: India's LRLACM and the Economics of the High-Low Missile Mix"
date: 2026-06-24
math: false
---

*On 15 June 2026, DRDO test-fired a cruise missile built to fly slower than a passenger jet, while India already operates one of the fastest cruise missiles in service anywhere. The contradiction isn't an oversight. It's the design brief.*

When a country tests a new missile, the instinct is to ask how fast it goes and how far it reaches, and to treat the bigger numbers as the better ones. The Long Range Land Attack Cruise Missile (LRLACM), which the Defence Research and Development Organisation flight-tested off the Odisha coast on 15 June 2026, breaks that instinct in a useful way. It is deliberately subsonic, cruising somewhere around Mach 0.7 to 0.8, at a time when India already fields the BrahMos, widely regarded as the fastest supersonic cruise missile in operational service. So why build a slow missile when you've already solved fast?

That question turns out to be the most interesting thing about the program, and the answer says more about how long-range strike actually works than any single line on a spec sheet.

## What actually happened on 15 June

The test ran from Dr APJ Abdul Kalam Island, the former Wheeler Island, with tracking handled by the Integrated Test Range at Chandipur. The Ministry of Defence reported that the missile met all mission objectives. Its release singled out two things: the indigenous Manik turbofan that sustains the cruise phase, and the navigation stack, a Ring Laser Gyroscope inertial system backed by GPS and India's own NavIC constellation, with terrain-contour matching for flying low.

One detail is worth getting right, because a lot of the coverage blurs it. This was the *second* flight test, not the debut. The maiden flight was on 12 November 2024, also from Chandipur, off a mobile articulated launcher. So 15 June was a repeat-and-extend, and the program is moving toward induction without being there yet. DRDO has been explicit that more trials come before the missile is cleared for production.

The nodal laboratory is the Aeronautical Development Establishment in Bengaluru, with Bharat Dynamics and Bharat Electronics as development-cum-production partners. The lineage runs back through the Nirbhay subsonic cruise missile, first tested in 2013 on an imported Russian engine, and the Indigenous Technology Cruise Missile demonstrator that existed largely to prove out the Manik. The LRLACM is what you get when that decade of work finally gets productised.

## Why "slow" buys you almost everything else

Here is the part that rewards an engineer's attention. The speed gap between the LRLACM and the BrahMos isn't a standalone number. It cascades into nearly every other spec, because the two missiles breathe air in fundamentally different ways.

BrahMos runs a liquid-fuelled ramjet. A ramjet has no compressor and no turbine, no moving parts in the airflow at all. It works by using the vehicle's own forward speed to ram incoming air into the combustion chamber and compress it before ignition. That's elegant, and it's also why a ramjet can't even start until the missile is already moving fast, which is what the solid rocket booster is for: it gets BrahMos up to speed before the ramjet lights. The penalty is thermodynamic. Holding Mach 3 against atmospheric drag burns propellant at a ferocious rate, so most of the airframe's internal volume has to be fuel. Add the dense alloys needed to survive the skin heating of supersonic flight and you end up with a heavy missile (around three tonnes), a short reach (the baseline was 290 km), and only enough mass budget left for a 200–300 kg warhead.

The LRLACM runs a turbofan, the Manik, producing roughly 425 kgf of thrust, about 4.2 kN. A turbofan diverts a large fraction of its intake air around the hot core. At subsonic speed that bypass flow is far more fuel-efficient than a ramjet screaming along at Mach 3, which is the same reason airliners use turbofans and not rockets. Low fuel burn buys range on a modest tank: the LRLACM is credited with 1,000 km or more, and several outlets cite up to 1,500 km. The bypass air earns its keep a second way too, by diluting and cooling the exhaust plume, which lowers the missile's infrared signature and makes it harder to track thermally.

So the chain is: choose subsonic, use a turbofan, get low fuel burn, and out the other end come long range, a lighter airframe (about a tonne), a cooler exhaust, and enough leftover mass for a heavier warhead, reported at roughly 400–450 kg (with a caveat on that figure below). "Slow" is the price you pay to collect all of that at once. It's a coherent bargain, not a compromise.

## The two missiles, side by side

| | LRLACM | BrahMos |
|---|---|---|
| **Speed** | Subsonic, ~Mach 0.7–0.8 | Supersonic, ~Mach 2.8–3.0 |
| **Engine** | Indigenous Manik turbofan (+ solid booster on surface launch) | Solid booster + liquid-fuelled ramjet |
| **Range** | ~1,000 km (official framing); up to 1,500 km (reported) | 290 km original; ~450 km extended-range; 800 km variant tested |
| **Warhead** | ~400–450 kg reported (unconfirmed) | 200–300 kg |
| **Mass / size** | ~1 t, ~6 m × 0.52 m | ~3 t, ~8.4 m × 0.6 m |
| **Origin** | Fully indigenous, engine included | Indo-Russian JV, P-800 Oniks heritage |
| **Flight profile** | Low-altitude terrain-following, loiter, waypoints | High-altitude dash, sea-skimming terminal dive |
| **Per-unit cost** | ~₹25 cr / $1–1.5M (unofficial estimate) | ~₹34 cr / $4.85M, ER naval (from an official contract) |
| **Primary role** | Long-range deep land strike | Anti-ship and precision land attack |

A word on reading that table: the BrahMos figures are mostly firm, because it's a fielded, exported, decades-old system. Several of the LRLACM figures are not. They're journalistic estimates DRDO hasn't confirmed, and I'll come back to which is which.

## Two ways to beat an air defence

The missiles don't only fly differently. They survive differently.

BrahMos survives by collapsing the defender's clock. At Mach 3 it covers roughly a kilometre a second, so a defender who first sees it at 50 km has well under a minute to detect it, classify it, generate a firing solution, and get an interceptor off the rail. There's a widely repeated claim from Operation Sindoor in May 2025, attributed to a Pakistani official, Rana Sanaullah, that defenders had only 30 to 45 seconds to even work out what an incoming BrahMos was. Treat the figure as a reported statement rather than a verified measurement, but the underlying physics holds: supersonic speed is itself a form of defence suppression. And because the airframe arrives at three tonnes and a kilometre per second, it dumps enormous kinetic energy on impact, which is why a "modest" warhead is still brutal against ships and hardened structures.

The LRLACM can't win that race. An interceptor will always be faster than a subsonic cruise missile, so the LRLACM doesn't race. It hides. Flying as low as around 50 m, it sits below the radar horizon of ground-based sensors and uses terrain (hills, tree lines, sea clutter) to break the line of sight. With terrain-contour matching it doesn't have to fly straight either; it can thread waypoints, skirt known radar sites, and arrive from a bearing nobody was watching. It can even loiter and wait for a target to be confirmed before committing. Survivability here comes from not being seen until the last few seconds, not from being too fast to hit.

Field both, and an adversary inherits a genuinely awkward problem. A defence tuned to catch a high-altitude Mach 3 dash is the wrong defence for a subsonic threat creeping through ground clutter, and the reverse is just as true.

## The real argument is economic

Speed and stealth are the visible differences. The decisive one is cost.

A supersonic ramjet missile is expensive to build: exotic alloys, imported engine components, tight thermal tolerances. The best-sourced number for BrahMos comes from the defence journalist Ajai Shukla, who in 2022 worked out, from a photographed Ministry of Defence contract, that the extended-range naval variant runs about ₹34 crore, roughly $4.85 million, per missile. The air-launched version costs more still.

Now picture spending a five-million-dollar weapon to flatten an ammunition dump, a fuel depot, or a communications relay. Those are soft, cheap targets, and the math is upside down: you run out of expensive missiles long before the enemy runs out of cheap things to defend. That's the attrition trap, and it shapes every long war.

The LRLACM is meant to fix the exchange ratio. Built domestically, skipping the premium supersonic engineering, it's expected to cost a fraction as much. Unofficial estimates land near ₹25 crore, about $1–1.5 million, though no official per-unit price exists. For scale, the American Tomahawk, the textbook subsonic land-attack missile, came in around $2 million in FY2022. A weapon in that bracket is cheap enough to fire in quantity.

That's the "high-low mix." You keep the small, premium BrahMos inventory for the targets that justify it, warships, buried command posts, movers you have to hit in the next sixty seconds, and you spend the cheaper LRLACM in volume to saturate air defences, crater runways, and grind down supply lines. The point of the LRLACM isn't that it beats BrahMos. It's that it lets you stop spending BrahMos on problems that don't deserve it.

## What we actually know, and what we don't

Confident spec sheets are everywhere, so it's worth separating the load-bearing facts from the estimates.

Confirmed, by official releases and multiple credible outlets: the 15 June 2026 test and its date; that it was the second flight, after November 2024; the indigenous Manik turbofan; the ADE / BDL / BEL development structure; the Nirbhay and ITCM lineage; ground and ship (UVLM) launch, with an air-launched Su-30MKI variant in development; and that both the Army and the Air Force have granted Acceptance of Necessity.

Not officially confirmed, and best cited as a range rather than a fact:

- **Range.** The official framing is "around 1,000 km." The popular "1,500 km" comes from secondary reporting. DRDO hasn't published a precise figure.
- **Warhead.** Reports say 400–450 kg; the Nirbhay heritage warhead was 200–300 kg. The real number is classified.
- **Cost and quantity.** The per-missile prices and unit counts circulating online are back-calculations from aggregate procurement approvals, not disclosed figures.
- **Nuclear capability.** Reported via Nirbhay heritage, but official LRLACM messaging stresses conventional deep strike and doesn't dwell on it.
- **The 2,500 km variant.** An ambition mentioned in some coverage, not a demonstrated capability.

PIB and MoD releases deliberately omit range, speed, and warhead specifics. That's standard for this class of weapon, and it's a good habit to assume any precise cruise-missile spec you read is an estimate until a government document says otherwise.

## Where this sits

Strip away the "game-changer" framing that tends to attach to these announcements and what's left is still real. The Manik matters on its own: it ends a long dependence on imported cruise-missile engines, which was the specific thing that held the Nirbhay program back for years. And a sovereign, long-range, terrain-following land-attack missile puts India in a small club of states that field one, alongside the US Tomahawk, Russia's Kalibr, China's CJ-10, and Pakistan's Babur.

It's worth being honest about the stage, though. Two successful tests is genuine progress, not an operational capability; induction still waits on further trials. The things actually worth watching next are the unglamorous ones: the induction timeline, whether the air-launched Su-30MKI integration pans out, a February 2026 request for information on a submarine-launched variant, and whether that 2,500 km ambition ever leaves the slide deck.

But the headline isn't the range or the speed. It's the logic. India looked at a strike arsenal built around one very fast, very expensive missile and decided the smart move was to also build a slow, cheap one. In a long war, the cheap one might be the one that matters.

---

*Sources: Ministry of Defence / PIB releases on the LRLACM flight tests (15 June 2026, PRID 2273160; maiden test 12 November 2024, PRID 2072829); Naval News (16 June 2026); reporting from The Tribune, India TV, and Asianet Newsable, 15–16 June 2026; Ajai Shukla's BrahMos unit-cost analysis, Business Standard (September 2022); GTRE Manik STFE specifications as reported via SPS Aviation; BrahMos figures via the manufacturer and standard references. Range, warhead, and cost figures for the LRLACM are journalistic estimates, not official confirmations.*
