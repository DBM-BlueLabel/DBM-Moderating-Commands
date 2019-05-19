{
  "name": "mute",
  "permissions": "NONE",
  "restriction": "1",
  "_id": "DhYvM",
  "actions": [
    {
      "member": "1",
      "varName": "",
      "permission": "MUTE_MEMBERS",
      "iftrue": "3",
      "iftrueVal": "2",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Check Member Permissions"
    },
    {
      "channel": "0",
      "varName": "",
      "message": "**ERROR:** You don't have permissions to use this command.\nRequired: `Mute Members` Permission.",
      "storage": "0",
      "varName2": "",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Send Message"
    },
    {
      "name": "End Action Sequence"
    },
    {
      "storage": "0",
      "varName": "",
      "name": "Delete Message"
    },
    {
      "info": "2",
      "infoIndex": "1",
      "storage": "1",
      "varName": "mentioned-member",
      "name": "Store Command Params"
    },
    {
      "info": "0",
      "infoIndex": "2",
      "storage": "1",
      "varName": "minutes",
      "name": "Store Command Params"
    },
    {
      "info": "1",
      "infoIndex": "3",
      "storage": "1",
      "varName": "reason",
      "name": "Store Command Params"
    },
    {
      "storage": "1",
      "varName": "mentioned-member",
      "comparison": "0",
      "value": "",
      "iftrue": "0",
      "iftrueVal": "2",
      "iffalse": "3",
      "iffalseVal": "2",
      "name": "Check Variable"
    },
    {
      "storage": "1",
      "varName": "minutes",
      "comparison": "0",
      "value": "",
      "iftrue": "0",
      "iftrueVal": "3",
      "iffalse": "3",
      "iffalseVal": "1",
      "name": "Check Variable"
    },
    {
      "storage": "1",
      "varName": "reason",
      "comparison": "0",
      "value": "",
      "iftrue": "3",
      "iftrueVal": "2",
      "iffalse": "0",
      "iffalseVal": "2",
      "name": "Check Variable"
    },
    {
      "channel": "0",
      "varName": "",
      "message": "**Wrong Format:**\nmute <@MentionMember> <minutes> <reason>",
      "storage": "0",
      "varName2": "",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Send Message"
    },
    {
      "name": "End Action Sequence"
    },
    {
      "storage": "1",
      "varName": "minutes",
      "comparison": "3",
      "value": "1",
      "iftrue": "0",
      "iftrueVal": "2",
      "iffalse": "3",
      "iffalseVal": "2",
      "name": "Check Variable"
    },
    {
      "channel": "0",
      "varName": "",
      "message": "**ERROR:** The number of minutes must be greater than 1.",
      "storage": "0",
      "varName2": "",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Send Message"
    },
    {
      "name": "End Action Sequence"
    },
    {
      "info": "1",
      "find": "Muted",
      "storage": "1",
      "varName": "mute-role",
      "name": "Find Role"
    },
    {
      "storage": "1",
      "varName": "mute-role",
      "comparison": "0",
      "value": "1",
      "iftrue": "3",
      "iftrueVal": "2",
      "iffalse": "0",
      "iffalseVal": "2",
      "name": "Check Variable"
    },
    {
      "channel": "0",
      "varName": "",
      "message": "**ERROR:** The mute role isn't exists.",
      "storage": "0",
      "varName2": "",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Send Message"
    },
    {
      "name": "End Action Sequence"
    },
    {
      "member": "1",
      "varName": "",
      "info": "7",
      "storage": "1",
      "varName2": "author-highest-role",
      "name": "Store Member Info"
    },
    {
      "member": "0",
      "varName": "",
      "info": "7",
      "storage": "1",
      "varName2": "mentioned-highest-role",
      "name": "Store Member Info"
    },
    {
      "role": "3",
      "varName": "author-highest-role",
      "info": "4",
      "storage": "1",
      "varName2": "author-role-position",
      "name": "Store Role Info"
    },
    {
      "role": "3",
      "varName": "mentioned-highest-role",
      "info": "4",
      "storage": "1",
      "varName2": "mentioned-role-position",
      "name": "Store Role Info"
    },
    {
      "storage": "1",
      "varName": "author-role-position",
      "comparison": "3",
      "value": "tempVars(\"mentioned-role-position\")",
      "iftrue": "0",
      "iftrueVal": "",
      "iffalse": "3",
      "iffalseVal": "2",
      "name": "Check Variable"
    },
    {
      "channel": "0",
      "varName": "",
      "message": "**ERROR:** You can't mute a member with highest role than yours.",
      "storage": "0",
      "varName2": "",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Send Message"
    },
    {
      "name": "End Action Sequence"
    },
    {
      "member": "0",
      "varName": "",
      "role": "3",
      "varName2": "mute-role",
      "iftrue": "0",
      "iftrueVal": "",
      "iffalse": "3",
      "iffalseVal": "2",
      "name": "Check If Member has Role"
    },
    {
      "channel": "0",
      "varName": "",
      "message": "**ERROR:** The member already in mute.",
      "storage": "0",
      "varName2": "",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Send Message"
    },
    {
      "name": "End Action Sequence"
    },
    {
      "member": "0",
      "varName2": "",
      "role": "3",
      "varName": "mute-role",
      "name": "Add Member Role"
    },
    {
      "title": "Member Muted",
      "author": "${member.displayName}",
      "color": "ff0000",
      "timestamp": "true",
      "url": "",
      "authorIcon": "${msg.author.displayAvatarURL}",
      "imageUrl": "",
      "thumbUrl": "",
      "storage": "1",
      "varName": "mute-embed",
      "name": "Create Embed Message"
    },
    {
      "storage": "1",
      "varName": "mute-embed",
      "message": "${member} mute ${mentionedUser} for **${tempVars(\"minutes\")}** minutes.",
      "name": "Set Embed Description"
    },
    {
      "storage": "1",
      "varName": "mute-embed",
      "fieldName": "Reason",
      "message": "${tempVars(\"reason\")}",
      "inline": "1",
      "name": "Add Embed Field"
    },
    {
      "storage": "1",
      "varName": "mute-embed",
      "channel": "0",
      "varName2": "",
      "storage3": "0",
      "varName3": "",
      "name": "Send Embed Message"
    },
    {
      "storage": "1",
      "varName": "mute-embed",
      "channel": "2",
      "varName2": "",
      "storage3": "0",
      "varName3": "",
      "name": "Send Embed Message"
    },
    {
      "storage": "2",
      "varName": "mute-log-channel",
      "comparison": "0",
      "value": "",
      "iftrue": "0",
      "iftrueVal": "",
      "iffalse": "3",
      "iffalseVal": "1",
      "name": "Check Variable"
    },
    {
      "storage": "1",
      "varName": "mute-embed",
      "channel": "6",
      "varName2": "mute-log-channel",
      "storage3": "0",
      "varName3": "",
      "name": "Send Embed Message"
    },
    {
      "time": "${tempVars(\"minutes\")}",
      "measurement": "2",
      "name": "Wait"
    },
    {
      "member": "0",
      "varName": "",
      "role": "3",
      "varName2": "mute-role",
      "iftrue": "0",
      "iftrueVal": "",
      "iffalse": "1",
      "iffalseVal": "",
      "name": "Check If Member has Role"
    },
    {
      "member": "0",
      "varName2": "",
      "role": "3",
      "varName": "mute-role",
      "name": "Remove Member Role"
    },
    {
      "title": "Member Unmuted Automatically",
      "author": "${tempVars(\"mentioned-member\").displayName}",
      "color": "00ff00",
      "timestamp": "true",
      "url": "",
      "authorIcon": "${tempVars(\"mentioned-member\").user.displayAvatarURL}",
      "imageUrl": "",
      "thumbUrl": "",
      "storage": "1",
      "varName": "unmute-embed",
      "name": "Create Embed Message"
    },
    {
      "storage": "1",
      "varName": "unmute-embed",
      "message": "${mentionedUser} unmuted automatically after ${tempVars(\"minutes\")} minutes.",
      "name": "Set Embed Description"
    },
    {
      "storage": "1",
      "varName": "unmute-embed",
      "fieldName": "Moderator",
      "message": "${member.displayName}",
      "inline": "0",
      "name": "Add Embed Field"
    },
    {
      "storage": "1",
      "varName": "unmute-embed",
      "fieldName": "Reason",
      "message": "${tempVars(\"reason\")}",
      "inline": "0",
      "name": "Add Embed Field"
    },
    {
      "storage": "1",
      "varName": "unmute-embed",
      "channel": "0",
      "varName2": "",
      "storage3": "0",
      "varName3": "",
      "name": "Send Embed Message"
    },
    {
      "storage": "1",
      "varName": "unmute-embed",
      "channel": "2",
      "varName2": "",
      "storage3": "0",
      "varName3": "",
      "name": "Send Embed Message"
    },
    {
      "storage": "2",
      "varName": "mute-log-channel",
      "comparison": "0",
      "value": "",
      "iftrue": "0",
      "iftrueVal": "",
      "iffalse": "1",
      "iffalseVal": "",
      "name": "Check Variable"
    },
    {
      "storage": "1",
      "varName": "unmute-embed",
      "channel": "6",
      "varName2": "mute-log-channel",
      "storage3": "0",
      "varName3": "",
      "name": "Send Embed Message"
    }
  ]
}
