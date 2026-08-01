<script>
    import { dues } from '$lib/utils/helper';
    let one, oneOne, oneOneOne, oneTwo, oneTwoOne, oneTwoTwo, oneTwoThree, oneTwoFour, oneTwoFive, oneThree;
    let two, twoOne, twoTwo, twoThree;
    let three, threeOne;
    let four, fourOne, fourTwo;
    let five, fiveOne;
    let six, sixOne, sixTwo, sixThree;
    let seven, sevenOne, sevenTwo, sevenThree;

    const goToSection = (section) => {
        const top = section.getBoundingClientRect().top + window.pageYOffset;
        window.scrollTo({left: 0, top, behavior: 'smooth'});
    }
</script>

<style>
    .constitution {
        position: relative;
        z-index: 1;
        width: 92%;
        max-width: 800px;
        margin: 8em auto 10em;
    }

    h1 {
        font-size: 2em;
        line-height: 1.2em;
        text-align: center;
        margin: 2em 0 1.5em;
    }

    h2 {
        font-size: 1.5em;
        line-height: 1.2em;
    }

    h3 {
       /* text-decoration: underline;*/
        font-size: 1.3em;
        line-height: 1.2em;
    }

    h4 {
        text-decoration: underline;
        margin-left: 2em;
        font-size: 1.2em;
        line-height: 1.2em;
    }

    h5 {
        margin-left: 6em;
        font-size: 0.8em;
        line-height: 1.1em;
    }

    .subBlock {
        margin-left: 2.4em;
    }

    .sectionHeading {
        margin: 4em 0 1.5em;
    }

    .subSectionHeading {
        margin: 1.5em 0 1.5em;
    }

    .underscore {
        text-decoration: underline;
    }

    .right {
        text-align: right;
    }

    .positionMaximums td {
        min-width: 3em;
    }

    .noUnderscore {
        text-decoration: none;
    }

    .clickable {
        cursor: pointer;
    }

    .clickable:hover {
        color: #00316b;
    }

    /*p {
        color: #000;
    }*/
</style>

<div class="constitution">
    <h1 class="noUnderscore">Night Fishin’ League Constitution</h1>
    
    <h2 class="noUnderscore">TABLE OF CONTENTS</h2>
    
    <h4 class="noUnderscore clickable" onclick={() => goToSection(one)}>Section 1: League Profile</h4>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(two)}>Section 2: League Rules</h4>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(three)}>Section 3: Scoring Settings</h4>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(four)}>Section 4: League Fees</h4>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(five)}>Section 5: Co-Owners, Divisions, League Schedule & Playoff Setting</h4>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(six)}>Section 6: Trophy & Roster</h4>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(seven)}>Section 7: League Keepers & Draft</h4>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(eight)}>Section 8: Draft Order</h4>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(nine)}>Section 9: League Calendar & Rule Changes</h4>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(ten)}>Section 10: Special COVID Rules for 2020 Season</h4>

    

    <hr />
    
    <h2 class="sectionHeading" bind:this={one}>Section 1: League Profile</h2>
    
    <h3>League Name  – Night Fishin League</h3>
    <h3>Commissioner – Steven Gross (2013-Present)</h3>
    <ul>
            <li>In charge of arranging draft party and festivities included with it</li>
    </ul>
    <h3>Draft Superintendent – Cameron Parker</h3>
    <ul>
            <li>In charge of arranging draft party and festivities included with it</li>
    </ul>
    <h3>Director of Trophies – Matthew Halton</h3>
    <ul>
            <li>In charge of current and future trophy matters</li>
    </ul>
    <h3>Director of Divisional Forecasting & Parlay Strategy – OPEN</h3>
    <ul>
            <li>In charge of placing a unified parlay bet of NFL divisional winners on behalf of the league</li>
    </ul>
    <p>*Granted Co-Commissioner Controls</p>
    
    
    <h2 class="sectionHeading" bind:this={two}>Section 2: League Rules</h2>

    <p>Undroppable List: None</p>
<p>Max Adds per Season: No</p>
<p>Max Adds per Week: No</p>
<p>Max Trades per Season: No</p>
<p>Trade Review Type: No Review - Commish can reverse action on outlandish trades</p>
<p>Trade Deadline: Week 11</p>
<p>Waiver Period: 1 day</p>
<p>Waiver Type: FAAB ($100) - FAAB is tradable</p>
<p>Free Agent Lock Type: Yes (player locks at game time)</p>
<p>Start of Season: Week 1</p>
<p>Keeper Settings: 5 Keepers</p>
<p>Keeper Lock Date: Exactly 1 week before league draft</p>
<p>Standings Tiebreaker:</p>
<p>

    1.      Divisional Record
</p>
<p>

    2.      Head to Head Record
</p>
<p>

    3.      Total Points
</p>
<p>Allow Matchup Ties: Yes</p>
<p>Allow Draft Pick Trades: Teams may make trades for picks in the upcoming year. The only period at which trades for the current year and upcoming year can be made at the same time is during the draft. </p>

<h2 class="sectionHeading" bind:this={three}>Section 3: Scoring Settings</h2>
<h4>Offense – Passing</h4>
<p>
Passing Yards: 1 point for every 25 yards
</p>
<p>
Passing Touchdowns: 4 points
</p>
<p>
Interceptions Thrown: -2 points
</p>
<h4>
Offense – Rushing/Receiving
</h4>
<p>
Rushing/Receiving Yards: 1 point for every 10 yards
</p>
<p>
Rushing/Receiving Touchdowns: 6 points
</p>
<p>
 
</p>
<h4>
Offense – Miscellaneous
</h4>
<p>
Fumble Recovered for a Touchdown: 6 points
</p>
<p>
2 Point Conversion: 2 points
</p>
<p>
Fumbles Lost: -2 points
</p>
<p>
** Marginal points are used for offensive yardage
</p>
<h4>
Kicking
</h4>
<p>
PAT Made: 1 point
</p>
<p>
FG Made 0-49: 3 points
</p>
<p>
FG Made 50+: 5 points
</p>
<h4>
Defense/Special Teams
</h4>
<p>
Sacks: 1 point
</p>
<p>
Interceptions: 2 points
</p>
<p>
Fumbles Recovered: 2 points
</p>
<p>
Safeties: 2 points
</p>
<p>
Touchdowns: 6 points
</p>
<p>
Kickoff and Punt Return Touchdowns: 6 points
</p>
<p>
0 Points Allowed: 10 points
</p>
<p>
1-6 Points Allowed: 7 points
</p>
<p>
7-13 Points Allowed: 4 points
</p>
<p>
14-20 Points Allowed: 1 point
</p>
<p>
21-27 Points Allowed: 0 points
</p>
<p>
28-34 Points Allowed: -1 point
</p>
<p>
35+ Points Allowed: -4 points
</p>
    

    <ol>
        <li>Points For</li>
        <li>Head 2 Head Record</li>
        <li>Division Record</li>
        <li>Total Points Against</li>
        <li>Coin Flip</li>
        <li>Duel to the death</li>
    </ol>

    <h2 class="sectionHeading" bind:this={five}>Section 5 Tanking Policy</h2>

</div>
