---
description: Everything you need to know about how to setup and use Watora's blindtest.
---

# Blindtest

## Introduction

A blindtest is a game where you have to guess the name of the song that’s currently playing. With Watora you can play this famous game on Discord by starting a blindtest game and directly sending the song title to your channel. It's easy and highly configurable.

## Starting a blindtest

To start a blindtest you will have to use `blindtest` \(or `bt`\)

<table>
  <thead>
    <tr>
      <th style="text-align:left">Usage</th>
      <th style="text-align:left">Help</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><b><code>blindtest anime (other_options)</code></b>
      </td>
      <td style="text-align:left">Starts a blindtest with the most popular anime songs.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p><b><code>blindtest mal=username,</code></b>
        </p>
        <p><b><code>username_two,... (other_options)</code></b>
        </p>
      </td>
      <td style="text-align:left">
        <p>Start a blindtest with the anime from the username’s MyAnimeList.</p>
        <p>You can load several anime lists at once by separating usernames with
          commas.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>blindtest autoplaylist=name (other_options)</code></b>
      </td>
      <td style="text-align:left">Starts a blindtest with the songs of an autoplaylist.</td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>blindtest difficulty=[0-6] (other_options)</code></b>
      </td>
      <td style="text-align:left">
        <p>Start a blindtest using the MyAnimeList top listed anime and set a 
          difficulty level.
          <br />Value must be between 0 and 6.</p>
        <p>Difficulty 0 uses the same list as <code>bt anime</code></p>
        <p><em>Example: difficulty 3 means that all anime in MyAnimeList top from 1 to 600 are loaded.</em>
        </p>
      </td>
    </tr>
  </tbody>
</table>## Options

<table>
  <thead>
    <tr>
      <th style="text-align:left">Name</th>
      <th style="text-align:left">Default</th>
      <th style="text-align:left">Help</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><b><code>longestword</code></b>
      </td>
      <td style="text-align:left"><code>false</code>
      </td>
      <td style="text-align:left">
        <p>Accept the longest word as a good answer.</p>
        <p><em>Accepted values: true or false</em>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>listening</code></b>
      </td>
      <td style="text-align:left"><code>false</code>
      </td>
      <td style="text-align:left">
        <p>Do not accept answers, remove the timeout, and just listen to the songs.</p>
        <p><em>Accepted values: true or false</em>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>timeout</code></b>
      </td>
      <td style="text-align:left"><code>120</code>
      </td>
      <td style="text-align:left">Timeout before stopping the song if not found.
        <br /><em>Value must be between 3 and 300 seconds</em>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>severity</code></b>
      </td>
      <td style="text-align:left"><code>100</code>
      </td>
      <td style="text-align:left">
        <p>Degree of match between answer and title.</p>
        <p><em>Value must be between 1 and 100%</em>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>percentage</code></b>
      </td>
      <td style="text-align:left"><code>100,0,0</code>
      </td>
      <td style="text-align:left">Percentage of OP, ED, OST.
        <br /><em>The sum of all values should be 100.</em>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>wait</code></b>
      </td>
      <td style="text-align:left"><code>5</code>
      </td>
      <td style="text-align:left">Time to wait before each song.
        <br /><em>Value must be between</em> 0 and 30 seconds.</td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>argument</code></b>
      </td>
      <td style="text-align:left"><code>all</code>
      </td>
      <td style="text-align:left">Only select a type of watched anime in the given anime lists.
        <br /><em>Accepted values: all, completed, watching, onhold, dropped, ptw.</em>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>remove</code></b>
      </td>
      <td style="text-align:left"><code>ptw</code>
      </td>
      <td style="text-align:left">
        <p>Ignore a type (or serveral) of watched anime (separated by commas) in
          the given anime lists.</p>
        <p><em>Accepted values: completed, watching, onhold, dropped, ptw, nothing.</em>
        </p>
      </td>
    </tr>
  </tbody>
</table>{% hint style="info" %}
Add your settings in a [Custom Command](custom-commands.md) to start your favorite blindtest as fast as possible.
{% endhint %}

## Points

When you guess the right answer, you earn points. You can earn up to 3 points per right answer. The server's ranking can be displayed with `btrank`

| Points | Accuracy |
| :--- | :--- |
| 1 | Normal right answer \(based on options, or synonyms...\) |
| 2 | Answer matched the main name with the same special characters. |
| 3 | Answer matches the main name with the same special characters, uppercase and lowercase. |

## Examples

**`bt mal=zenrac percentage=50,50,0 remove=ptw,dropped`**  
Starts a blindtest from Zenrac's MyAnimeList, with 50% of Opening and 50% of Ending, without adding the “plan to watch” and “dropped anime” from the list.  


**`bt mal=zenrac,razmoute argument=dropped`**  
Starts a blindtest from Zenrac's MyAnimeList and Razmoute's MyAnimeList, adding only the dropped anime from both lists.

