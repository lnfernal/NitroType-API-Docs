# NitroType API Docs (🚧 Under Construction 🚧)
Documentation for the unofficial NitroType API

----

## Base URL
`https://www.nitrotype.com/api/`

----

## Endpoints

  * [Achievements](#achievements)
  * [Auth](#auth)
  * [Cars](#cars)
  * [Classes](#classes)
  * [Friends](#friends)
  * [Items](#items)
  * [News](#news)
  * [Players](#players)
  * [Purchase](#purchase)
  * [Race](#race)
  * [Referrals](#referrals)
  * [Rewards](#rewards)
  * [Scoreboard](#scoreboard)
  * [Settings](#settings)
  * [Stats](#stats)
  * [Teams](#teams)
  * [Miscellaneous](#miscellaneous)

## Achievements

## Auth

## Cars

## Classes

## Friends

## Items

## News

## Players

## Purchase

## Race

## Referrals

## Rewards

## Scoreboard

## Settings

## Stats

## Teams
  * [`<???>/invite`](#teams???invite)
  * [`<tag>`](#teamstag)
  * [`<teamID>/accept-invite`](#teamsteamidaccept-invite)
  * [`<teamID>/apply`](#teamsteamidapply)
  * [`<teamId>/ignore-invite`](#teamsteamidignore-invite)
  * [`applications`](#teamsapplications)
  * [`boost`](#teamsboost)
  * [`create`](#teamscreate)
  * [`delete`](#teamsdelete)
  * [`leave`](#teamsleave)
  * [`motd`](#teamsmotd)
  * [`search`](#teamssearch)
  * [`update`](#teamsupdate)

### <code>teams/\<???>/invite</code>
???

<table>
	<tr>
	<th>method</th>
	<th>uhash</th>
	<th>apiScope</th>
	</tr>
	<tr>
	<td>POST</td>
	<td><code>false</code></td>
	<td><code>"???"</code></td>
	</tr>
</table>

### <code>teams/\<tag></code>
Fetch information from a team.

<table>
	<tr>
	<th>method</th>
	<th>uhash</th>
	<th>apiScope</th>
	</tr>
	<tr>
	<td>GET</td>
	<td><code>true</code></td>
	<td><code>"fetchDetails"</code></td>
	</tr>
</table>

### <code>teams/\<teamID>/accept-invite</code>
Accept a team invite.

<table>
	<tr>
	<th>method</th>
	<th>uhash</th>
	<th>apiScope</th>
	</tr>
	<tr>
	<td>POST</td>
	<td><code>true</code></td>
	<td><code>"acceptTeamInvite"</code></td>
	</tr>
</table>

### <code>teams/\<teamID>/apply</code>
Apply for a team.

<table>
	<tr>
	<th>method</th>
	<th>uhash</th>
	<th>apiScope</th>
	</tr>
	<tr>
	<td>POST</td>
	<td><code>true</code></td>
	<td><code>"applyForTeam"</code></td>
	</tr>
</table>

### <code>teams/\<teamId>/ignore-invite</code>
Ignore a team invite.

<table>
	<tr>
	<th>method</th>
	<th>uhash</th>
	<th>apiScope</th>
	</tr>
	<tr>
	<td>POST</td>
	<td><code>true</code></td>
	<td><code>"ignoreTeamInvite"</code></td>
	</tr>
</table>

### <code>teams/applications</code>
Fetch team applications.

<table>
	<tr>
	<th>method</th>
	<th>uhash</th>
	<th>apiScope</th>
	</tr>
	<tr>
	<td>GET</td>
	<td><code>true</code></td>
	<td><code>"fetchApplications"</code></td>
	</tr>
</table>

### <code>teams/boost</code>
Add a reaction (boost) to a motd.

<table>
	<tr>
	<th>method</th>
	<th>uhash</th>
	<th>apiScope</th>
	</tr>
	<tr>
	<td>POST</td>
	<td><code>true</code></td>
	<td><code>"addMotdBoost"</code></td>
	</tr>
</table>

**Params:** boostID, teamMotdID

### <code>teams/create</code>
Create a team.

<table>
	<tr>
	<th>method</th>
	<th>uhash</th>
	<th>apiScope</th>
	</tr>
	<tr>
	<td>POST</td>
	<td><code>true</code></td>
	<td><code>"createTeam"</code></td>
	</tr>
</table>

**Params:** tag, name, tagColor, minRaces, minSpeed, otherRequirements, password, enrollment, autoRemove

### <code>teams/delete</code>
Delete a team.

<table>
	<tr>
	<th>method</th>
	<th>uhash</th>
	<th>apiScope</th>
	</tr>
	<tr>
	<td>POST</td>
	<td><code>true</code></td>
	<td><code>"disbandTeam"</code></td>
	</tr>
</table>

**Params:** password

### <code>teams/leave</code>
Leave a team.

<table>
	<tr>
	<th>method</th>
	<th>uhash</th>
	<th>apiScope</th>
	</tr>
	<tr>
	<td>POST</td>
	<td><code>true</code></td>
	<td><code>"leaveTeam"</code></td>
	</tr>
</table>

### <code>teams/motd</code>
Post a message of the day (motd).

<table>
	<tr>
	<th>method</th>
	<th>uhash</th>
	<th>apiScope</th>
	</tr>
	<tr>
	<td>POST</td>
	<td><code>true</code></td>
	<td><code>"updateMOTD"</code></td>
	</tr>
</table>

**Params:** message

### <code>teams/search</code>
Search for teams.

<table>
	<tr>
	<th>method</th>
	<th>uhash</th>
	<th>apiScope</th>
	</tr>
	<tr>
	<td>GET</td>
	<td><code>true</code></td>
	<td><code>"teamSearch"</code></td>
	</tr>
</table>

**Params:** invites, racesPlayed, speed

### <code>teams/update</code>
Update a team.

<table>
	<tr>
	<th>method</th>
	<th>uhash</th>
	<th>apiScope</th>
	</tr>
	<tr>
	<td>POST</td>
	<td><code>true</code></td>
	<td><code>"editTeam"</code></td>
	</tr>
</table>

**Params:** tag, name, tagColor, minRaces, minSpeed, otherRequirements, password, enrollment, autoRemove

## Miscellaneous
