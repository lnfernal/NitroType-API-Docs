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
  * [`achievements/check`](#v2achievementscheck)
  * [`achievements/claim/<achievementID>`](#v2achievementsclaimachievementid)
  * [`achievements/extra`](#v2achievementsextra)

### <code>v2/achievements/check</code>
???

<table>
	<tr>
	<th>method</th>
	<th>uhash</th>
	<th>apiScope</th>
	</tr>
	<tr>
	<td>POST</td>
	<td><code>true</code></td>
	<td><code>"???"</code></td>
	</tr>
</table>

**Params:** ids

### <code>v2/achievements/claim/\<achievementID></code>
Claim an achievement.

<table>
	<tr>
	<th>method</th>
	<th>uhash</th>
	<th>apiScope</th>
	</tr>
	<tr>
	<td>GET</td>
	<td><code>true</code></td>
	<td><code>"claimAchievement"</code></td>
	</tr>
</table>

### <code>v2/achievements/extra</code>
???

<table>
	<tr>
	<th>method</th>
	<th>uhash</th>
	<th>apiScope</th>
	</tr>
	<tr>
	<td>POST</td>
	<td><code>true</code></td>
	<td><code>"???"</code></td>
	</tr>
</table>

**Params:** id

## Auth
  * [`auth/class-login/<sectionID>`](#v2authclass-loginsectionid)
  * [`auth/login/<???>`](#v2authlogin???)
  * [`auth/login/username`](#v2authloginusername)
  * [`auth/redirect/<facebook|google|clever>`](#v2authredirectfacebook|google|clever)
  * [`auth/register/username`](#v2authregisterusername)
  * [`auth/reset-password`](#v2authreset-password)
  * [`auth/reset-password/change`](#v2authreset-passwordchange)
  * [`auth/validate-captcha`](#v2authvalidate-captcha)
  * [`auth/validate-email`](#v2authvalidate-email)

### <code>v2/auth/class-login/\<sectionID></code>
Login to a class.

<table>
	<tr>
	<th>method</th>
	<th>uhash</th>
	<th>apiScope</th>
	</tr>
	<tr>
	<td>POST</td>
	<td><code>false</code></td>
	<td><code>"logInToClass"</code></td>
	</tr>
</table>

**Params:** sectionID

### <code>v2/auth/login/\<???></code>
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
	<td><code>"login"</code></td>
	</tr>
</table>

**Params:** ???, ...

### <code>v2/auth/login/username</code>
Login to an account.

<table>
	<tr>
	<th>method</th>
	<th>uhash</th>
	<th>apiScope</th>
	</tr>
	<tr>
	<td>POST</td>
	<td><code>false</code></td>
	<td><code>"login"</code></td>
	</tr>
</table>

**Params:** username, password, captchaToken, tz

### <code>v2/auth/redirect/\<facebook|google|clever></code>
Redirect to third-party login.

<table>
	<tr>
	<th>method</th>
	<th>uhash</th>
	<th>apiScope</th>
	</tr>
	<tr>
	<td>GET</td>
	<td><code>false</code></td>
	<td><code>"???"</code></td>
	</tr>
</table>

### <code>v2/auth/register/username</code>
Register (and qualify) an account.

<table>
	<tr>
	<th>method</th>
	<th>uhash</th>
	<th>apiScope</th>
	</tr>
	<tr>
	<td>POST</td>
	<td><code>false</code></td>
	<td><code>"signup"</code></td>
	</tr>
</table>

**Params:** username, password, email, acceptPolicy, receiveContact, tz, qualifying, avgSpeed, avgAcc, carID, raceSounds

### <code>v2/auth/reset-password</code>
Reset an account's password.

<table>
	<tr>
	<th>method</th>
	<th>uhash</th>
	<th>apiScope</th>
	</tr>
	<tr>
	<td>POST</td>
	<td><code>false</code></td>
	<td><code>"forgotPassword"</code></td>
	</tr>
</table>

**Params:** email

### <code>v2/auth/reset-password/change</code>
Reset an account's password.

<table>
	<tr>
	<th>method</th>
	<th>uhash</th>
	<th>apiScope</th>
	</tr>
	<tr>
	<td>POST</td>
	<td><code>true</code></td>
	<td><code>"resetPassword"</code></td>
	</tr>
</table>

**Params:** newPassword, newPassword2, userID, hash

### <code>v2/auth/validate-captcha</code>
Submit a captcha user response token.

<table>
	<tr>
	<th>method</th>
	<th>uhash</th>
	<th>apiScope</th>
	</tr>
	<tr>
	<td>POST</td>
	<td><code>false</code></td>
	<td><code>"validateCaptcha"</code></td>
	</tr>
</table>

**Params:** token

### <code>v2/auth/validate-email</code>
Verify an account's email address.

<table>
	<tr>
	<th>method</th>
	<th>uhash</th>
	<th>apiScope</th>
	</tr>
	<tr>
	<td>POST</td>
	<td><code>true</code></td>
	<td><code>"validateEmail"</code></td>
	</tr>
</table>

**Params:** hash, userID

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
