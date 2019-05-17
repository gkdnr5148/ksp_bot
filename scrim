import discord
import os
client = discord.Client()


@client.event
async def on_ready():
    print(client.user.id)
    print("ready")
    game = discord.Game("KSP_SCRIM BOT")
    await client.change_presence(status=discord.Status.online, activity=game)



@client.event
async def on_message(message):
    if message.content.startswith("!서버"):
        await message.channel.send("```도쿄GCE１```")
    if message.content.startswith("!안내"):
        await message.channel.send("@everyone 금일부터 시간표가 변경되었습니다.")
    if message.content.startswith("!카운트1"):
        await message.channel.send("a!scrim countdown  1 곧시작합니다.")

        
access_token = os.environ["BOT_TOKEN"]        
client.run(access_token)
