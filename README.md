repeat wait() until game:IsLoaded()

if _G.Team == "Pirate" then
	for i,v in pairs(getconnections(game:GetService("Players").LocalPlayer.PlayerGui.Main.ChooseTeam.Container.Pirates.Frame.ViewportFrame.TextButton.MouseButton1Click)) do
		v.Function()
	end
elseif _G.Team == "Marine" then
	for i,v in pairs(getconnections(game:GetService("Players").LocalPlayer.PlayerGui.Main.ChooseTeam.Container.Marines.Frame.ViewportFrame.TextButton.MouseButton1Click)) do
		v.Function()
	end
else
	for i,v in pairs(getconnections(game:GetService("Players").LocalPlayer.PlayerGui.Main.ChooseTeam.Container.Pirates.Frame.ViewportFrame.TextButton.MouseButton1Click)) do
		v.Function()
	end
end

wait(1)



local library = loadstring(game:HttpGet("https://raw.githubusercontent.com/zxciaz/VenyxUI/main/Reuploaded"))()
local venyx = library.new("COMMUNITY", 5012544693)
local page = venyx:addPage("Main", 5012544693) 
local section1 = page:addSection("AutoFarm")

--------------------5012544693

local placeId = game.PlaceId
Magnet = true
if placeId == 2753915549 then
    First_Sea = true
elseif placeId == 4442272183 then
    Second_Sea = true
elseif placeId == 7449423635 then
    Third_Sea = true
end

_G.FarmSwiish = true
spawn(function()
    while wait() do
        pcall(function()
        _G.FarmSwiish = true
        wait(3)
        _G.FarmSwiish = false
        wait(3)
        end)
    end
end)


function Click()
    game:GetService'VirtualUser':CaptureController()
    game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
end
function CheckLevel()
local MyLevel = game.Players.LocalPlayer.Data.Level.Value
if First_Sea then
    if MyLevel == 1 or MyLevel <= 9 then 
        Ms = "Bandit [Lv. 5]"
        QuestName = "BanditQuest1"
        QuestNumber = 1
        NameMon = "Bandit"
        CFrameQuest = CFrame.new(1060.9383544922, 16.455066680908, 1547.7841796875)
        CFrameMon = CFrame.new(1038.5533447266, 41.296249389648, 1576.5098876953)
    elseif MyLevel == 10 or MyLevel <= 14 then 
        Ms = "Monkey [Lv. 14]"
        QuestName = "JungleQuest"
        QuestNumber = 1
        NameMon = "Monkey"
        CFrameQuest = CFrame.new(-1604.12012, 36.8521118, 154.23732, 0.0648873374, -4.70858913e-06, -0.997892559, 1.41431883e-07, 1, -4.70933674e-06, 0.997892559, 1.64442184e-07, 0.0648873374)
        CFrameMon = CFrame.new(-1448.1446533203, 50.851993560791, 63.60718536377)
    elseif MyLevel == 15 or MyLevel <= 29 then 
        Ms = "Gorilla [Lv. 20]"
        QuestName = "JungleQuest"
        QuestNumber = 2
        NameMon = "Gorilla"
        CFrameQuest = CFrame.new(-1601.6553955078, 36.85213470459, 153.38809204102)
        CFrameMon = CFrame.new(-1142.6488037109, 40.462348937988, -515.39227294922)
    elseif MyLevel == 30 or MyLevel <= 39 then 
        Ms = "Pirate [Lv. 35]"
        QuestName = "BuggyQuest1"
        QuestNumber = 1
        NameMon = "Pirate"
        CFrameQuest = CFrame.new(-1140.1761474609, 4.752049446106, 3827.4057617188)
        CFrameMon = CFrame.new(-1201.0881347656, 40.628940582275, 3857.5966796875)
    elseif MyLevel == 40 or MyLevel <= 59 then 
        Ms = "Brute [Lv. 45]"
        QuestName = "BuggyQuest1"
        QuestNumber = 2
        NameMon = "Brute"
        CFrameQuest = CFrame.new(-1140.1761474609, 4.752049446106, 3827.4057617188)
        CFrameMon = CFrame.new(-1387.5324707031, 24.592035293579, 4100.9575195313)
    elseif MyLevel == 60 or MyLevel <= 74 then 
        Ms = "Desert Bandit [Lv. 60]"
        QuestName = "DesertQuest"
        QuestNumber = 1
        NameMon = "Desert Bandit"
        CFrameQuest = CFrame.new(896.51721191406, 6.4384617805481, 4390.1494140625)
        CFrameMon = CFrame.new(984.99896240234, 16.109552383423, 4417.91015625)
    elseif MyLevel == 75 or MyLevel <= 89 then 
        Ms = "Desert Officer [Lv. 70]"
        QuestName = "DesertQuest"
        QuestNumber = 2
        NameMon = "Desert Officer"
        CFrameQuest = CFrame.new(896.51721191406, 6.4384617805481, 4390.1494140625)
        CFrameMon = CFrame.new(1547.1510009766, 14.452038764954, 4381.8002929688)
    elseif MyLevel == 90 or MyLevel <= 99 then 
        Ms = "Snow Bandit [Lv. 90]"
        QuestName = "SnowQuest"
        QuestNumber = 1
        NameMon = "Snow Bandits"
        CFrameQuest = CFrame.new(1386.8073730469, 87.272789001465, -1298.3576660156)
        CFrameMon = CFrame.new(1356.3028564453, 105.76865386963, -1328.2418212891)
    elseif MyLevel == 100 or MyLevel <= 119 then 
        Ms = "Snowman [Lv. 100]"
        QuestName = "SnowQuest"
        QuestNumber = 2
        NameMon = "Snowman"
        CFrameQuest = CFrame.new(1386.8073730469, 87.272789001465, -1298.3576660156)
        CFrameMon = CFrame.new(1218.7956542969, 138.01184082031, -1488.0262451172)
    elseif MyLevel == 120 or MyLevel <= 149 then 
        Ms = "Chief Petty Officer [Lv. 120]"
        QuestName = "MarineQuest2"
        QuestNumber = 1
        NameMon = "Chief Petty Officer"
        CFrameQuest = CFrame.new(-5035.49609375, 28.677835464478, 4324.1840820313)
        CFrameMon = CFrame.new(-4931.1552734375, 65.793113708496, 4121.8393554688)
    elseif MyLevel == 150 or MyLevel <= 174 then 
        Ms = "Sky Bandit [Lv. 150]"
        QuestName = "SkyQuest"
        QuestNumber = 1
        NameMon = "Sky Bandit"
        CFrameQuest = CFrame.new(-4841.83447, 717.669617, -2623.96436)
        CFrameMon = CFrame.new(-4970.74219, 294.544342, -2890.11353)
    elseif MyLevel == 175 or MyLevel <= 224 then 
        Ms = "Dark Master [Lv. 175]"
        QuestName = "SkyQuest"
        QuestNumber = 2
        NameMon = "Dark Master"
        CFrameQuest = CFrame.new(-4841.83447, 717.669617, -2623.96436)
        CFrameMon = CFrame.new(-5220.58594, 430.693298, -2278.17456)
    elseif MyLevel == 225 or MyLevel <= 274 then 
        Ms = "Toga Warrior [Lv. 225]"
        QuestName = "ColosseumQuest"
        QuestNumber = 1
        NameMon = "Toga Warrior"
        CFrameQuest = CFrame.new(-1576.11743, 7.38933945, -2983.30762)
        CFrameMon = CFrame.new(-1779.97583, 44.6077499, -2736.35474)
    elseif MyLevel == 275 or MyLevel <= 299 then 
        Ms = "Gladiator [Lv. 275]"
        QuestName = "ColosseumQuest"
        QuestNumber = 2
        NameMon = "Gladiato"
        CFrameQuest = CFrame.new(-1576.11743, 7.38933945, -2983.30762)
        CFrameMon = CFrame.new(-1274.75903, 58.1895943, -3188.16309)
    elseif MyLevel == 300 or MyLevel <= 329 then 
        Ms = "Military Soldier [Lv. 300]"
        QuestName = "MagmaQuest"
        QuestNumber = 1
        NameMon = "Military Soldier"
        CFrameQuest = CFrame.new(-5316.55859, 12.2370615, 8517.2998)
        CFrameMon = CFrame.new(-5363.01123, 41.5056877, 8548.47266)
    elseif MyLevel == 300 or MyLevel <= 374 then 
        Ms = "Military Spy [Lv. 330]"
        QuestName = "MagmaQuest"
        QuestNumber = 2
        NameMon = "Military Spy"
        CFrameQuest = CFrame.new(-5316.55859, 12.2370615, 8517.2998)
        CFrameMon = CFrame.new(-5787.99023, 120.864456, 8762.25293)
    elseif MyLevel == 375 or MyLevel <= 399 then 
        Ms = "Fishman Warrior [Lv. 375]"
        QuestName = "FishmanQuest"
        QuestNumber = 1
        NameMon = "Fishman Warrior"
        CFrameQuest = CFrame.new(61122.5625, 18.4716396, 1568.16504)
        CFrameMon = CFrame.new(61163.8515625, 5.3073043823242, 1819.7841796875)
    elseif MyLevel == 400 or MyLevel <= 449 then 
        Ms = "Fishman Commando [Lv. 400]"
        QuestName = "FishmanQuest"
        QuestNumber = 2
        NameMon = "Fishman Commando"
        CFrameQuest = CFrame.new(61122.5625, 18.4716396, 1568.16504)
        CFrameMon = CFrame.new(61163.8515625, 5.3073043823242, 1819.7841796875)
    elseif MyLevel == 450 or MyLevel <= 474 then 
        Ms = "God's Guard [Lv. 450]"
        QuestName = "SkyExp1Quest"
        QuestNumber = 1
        NameMon = "God's Guards"
        CFrameQuest = CFrame.new(-4721.71436, 845.277161, -1954.20105)
        CFrameMon = CFrame.new(-4716.95703, 853.089722, -1933.925427)
    elseif MyLevel == 475 or MyLevel <= 524 then 
        Ms = "Shanda [Lv. 475]"
        QuestName = "SkyExp1Quest"
        QuestNumber = 2
        NameMon = "Shandas"
        CFrameQuest = CFrame.new(-7863.63672, 5545.49316, -379.826324)
        CFrameMon = CFrame.new(-7685.12354, 5601.05127, -443.171509)
    elseif MyLevel == 525 or MyLevel <= 549 then 
        Ms = "Royal Squad [Lv. 525]"
        QuestName = "SkyExp2Quest"
        QuestNumber = 1
        NameMon = "Royal Squad"
        CFrameQuest = CFrame.new(-7902.66895, 5635.96387, -1411.71802)
        CFrameMon = CFrame.new(-7685.02051, 5606.87842, -1442.729)
    elseif MyLevel == 550 or MyLevel <= 624 then 
        Ms = "Royal Soldier [Lv. 550]"
        QuestName = "SkyExp2Quest"
        QuestNumber = 2
        NameMon = "Royal Soldier"
        CFrameQuest = CFrame.new(-7902.66895, 5635.96387, -1411.71802)
        CFrameMon = CFrame.new(-7864.44775, 5661.94092, -1708.22351)
    elseif MyLevel == 625 or MyLevel <= 649 then 
        Ms = "Galley Pirate [Lv. 625]"
        QuestName = "FountainQuest"
        QuestNumber = 1
        NameMon = "Galley Pirate"
        CFrameQuest = CFrame.new(5254.60156, 38.5011406, 4049.69678)
        CFrameMon = CFrame.new(5595.06982, 41.5013695, 3961.47095)
    elseif MyLevel >= 650 then 
        Ms = "Galley Captain [Lv. 650]"
        QuestName = "FountainQuest"
        QuestNumber = 2
        NameMon = "Galley Captain"
        CFrameQuest = CFrame.new(5254.60156, 38.5011406, 4049.69678)
        CFrameMon = CFrame.new(5658.5752, 38.5361786, 4928.93506)
    end
end
if Second_Sea then
    if MyLevel == 700 or MyLevel <= 724 then 
        Ms = "Raider [Lv. 700]"
        QuestName = "Area1Quest"
        QuestNumber = 1
        NameMon = "Raider"
        CFrameQuest = CFrame.new(-424.080078, 73.0055847, 1836.91589)
        CFrameMon = CFrame.new(-737.026123, 39.1748352, 2392.57959)
    elseif MyLevel == 725 or MyLevel <= 774 then 
        Ms = "Mercenary [Lv. 725]"
        QuestName = "Area1Quest"
        QuestNumber = 2
        NameMon = "Mercenary"
        CFrameQuest = CFrame.new(-424.080078, 73.0055847, 1836.91589)
        CFrameMon = CFrame.new(-973.731995, 95.8733215, 1836.46936)
    elseif MyLevel == 775 or MyLevel <= 874 then 
        Ms = "Swan Pirate [Lv. 775]"
        QuestName = "Area2Quest"
        QuestNumber = 1
        NameMon = "Swan Pirate"
        CFrameQuest = CFrame.new(632.698608, 73.1055908, 918.666321)
        CFrameMon = CFrame.new(970.369446, 142.653198, 1217.3667)
    elseif MyLevel == 875 or MyLevel <= 899 then 
        Ms = "Marine Lieutenant [Lv. 875]"
        QuestName = "MarineQuest3"
        QuestNumber = 1
        NameMon = "Marine Lieutenant"
        CFrameQuest = CFrame.new(-2442.65015, 73.0511475, -3219.11523)
        CFrameMon = CFrame.new(-2913.26367, 73.0011826)
    elseif MyLevel == 900 or MyLevel <= 949 then 
        Ms = "Marine Captain [Lv. 900]"
        QuestName = "MarineQuest3"
        QuestNumber = 2
        NameMon = "Marine Captain"
        CFrameQuest = CFrame.new(-2442.65015, 73.0511475, -3219.11523)
        CFrameMon = CFrame.new(-1868.67688, 73.0011826, -3321.66333)
    elseif MyLevel == 950 or MyLevel <= 974 then 
        Ms = "Zombie [Lv. 950]"
        QuestName = "ZombieQuest"
        QuestNumber = 1
        NameMon = "Zombie"
        CFrameQuest = CFrame.new(-5492.79395, 48.5151672, -793.710571)
        CFrameMon = CFrame.new(-5634.83838, 126.067039, -697.665039)
    elseif MyLevel == 975 or MyLevel <= 999 then 
        Ms = "Vampire [Lv. 975]"
        QuestName = "ZombieQuest"
        QuestNumber = 2
        NameMon = "Vampire"
        CFrameQuest = CFrame.new(-5492.79395, 48.5151672, -793.710571)
        CFrameMon = CFrame.new(-6030.32031, 6.4377408, -1313.5564)
    elseif MyLevel == 1000 or MyLevel <= 1049 then 
        Ms = "Snow Trooper [Lv. 1000]"
        QuestName = "SnowMountainQuest"
        QuestNumber = 1
        NameMon = "Snow Trooper"
        CFrameQuest = CFrame.new(604.964966, 401.457062, -5371.69287)
        CFrameMon = CFrame.new(535.893433, 401.457062, -5329.6958)
    elseif MyLevel == 1050 or MyLevel <= 1099 then 
        Ms = "Winter Warrior [Lv. 1050]"
        QuestName = "SnowMountainQuest"
        QuestNumber = 2
        NameMon = "Winter Warrior"
        CFrameQuest = CFrame.new(604.964966, 401.457062, -5371.69287)
        CFrameMon = CFrame.new(1223.7417, 454.575226, -5170.02148)
    elseif MyLevel == 1100 or MyLevel <= 1124 then 
        Ms = "Lab Subordinate [Lv. 1100]"
        QuestName = "IceSideQuest"
        QuestNumber = 1
        NameMon = "Lab Subordinate"
        CFrameQuest = CFrame.new(-6060.10693, 15.9868021, -4904.7876)
        CFrameMon = CFrame.new(-5769.2041, 37.9288292, -4468.38721)
    elseif MyLevel == 1125 or MyLevel <= 1174 then 
        Ms = "Horned Warrior [Lv. 1125]"
        QuestName = "IceSideQuest"
        QuestNumber = 2
        NameMon = "Horned Warrior"
        CFrameQuest = CFrame.new(-6060.10693, 15.9868021, -4904.7876)
        CFrameMon = CFrame.new(-6400.85889, 24.7645149, -5818.63574)
    elseif MyLevel == 1175 or MyLevel <= 1199 then 
        Ms = "Magma Ninja [Lv. 1175]"
        QuestName = "FireSideQuest"
        QuestNumber = 1
        NameMon = "Magma Ninja"
        CFrameQuest = CFrame.new(-5431.09473, 15.9868021, -5296.53223)
        CFrameMon = CFrame.new(-5496.65576, 58.6890411, -5929.76855)
    elseif MyLevel == 1200 or MyLevel <= 1349 then 
        Ms = "Lava Pirate [Lv. 1200]"
        QuestName = "FireSideQuest"
        QuestNumber = 2
        NameMon = "Lava Pirate"
        CFrameQuest = CFrame.new(-5431.09473, 15.9868021, -5296.53223)
        CFrameMon = CFrame.new(-5169.71729, 34.1234779, -4669.73633)
    elseif MyLevel == 1350 or MyLevel <= 1374 then 
        Ms = "Arctic Warrior [Lv. 1350]"
        QuestName = "FrostQuest"
        QuestNumber = 1
        NameMon = "Arctic Warrior"
        CFrameQuest = CFrame.new(5669.43506, 28.2117786, -6482.60107)
        CFrameMon = CFrame.new(5995.07471, 57.3188477, -6183.47314)
    elseif MyLevel == 1375 or MyLevel <= 1424 then 
        Ms = "Snow Lurker [Lv. 1375]"
        QuestName = "FrostQuest"
        QuestNumber = 2
        NameMon = "Snow Lurker"
        CFrameQuest = CFrame.new(5669.43506, 28.2117786, -6482.60107)
        CFrameMon = CFrame.new(5518.00684, 60.5559731, -6828.80518)
    elseif MyLevel == 1425 or MyLevel <= 1449 then 
        Ms = "Sea Soldier [Lv. 1425]"
        QuestName = "ForgottenQuest"
        QuestNumber = 1
        NameMon = "Sea Soldier"
        CFrameQuest = CFrame.new(-3052.99097, 236.881363, -10148.1943)
        CFrameMon = CFrame.new(-3030.3696289063, 191.13464355469, -9859.7958984375)
    elseif MyLevel >= 1450 then 
        Ms = "Water Fighter [Lv. 1450]"
        QuestName = "ForgottenQuest"
        QuestNumber = 2
        NameMon = "Water Fighter"
        CFrameQuest = CFrame.new(-3052.99097, 236.881363, -10148.1943)
        CFrameMon = CFrame.new(-3436.7727050781, 290.52191162109, -10503.438476563)
    end
end
if Third_Sea then
    if MyLevel >= 1500 and MyLevel <= 1524 then
        Ms = "Pirate Millionaire [Lv. 1500]"
        QuestName = "PiratePortQuest"
        QuestNumber = 1
        NameMon = "Pirate Millionaire"
        CFrameQuest = CFrame.new(-290.074677, 42.9034653, 5581.58984)
        CFrameMon = CFrame.new(81.164993286133, 43.755737304688, 5724.7021484375)
    elseif MyLevel >= 1525 and MyLevel <= 1574 then
        Ms = "Pistol Billionaire [Lv. 1525]"
        QuestName = "PiratePortQuest"
        QuestNumber = 2
        NameMon = "Pistol Billionaire"
        CFrameQuest = CFrame.new(-290.074677, 42.9034653, 5581.58984)
        CFrameMon = CFrame.new(81.164993286133, 43.755737304688, 5724.7021484375)
    elseif MyLevel >= 1575 and MyLevel <= 1599 then
        Ms = "Dragon Crew Warrior [Lv. 1575]"
        QuestName = "AmazonQuest"
        QuestNumber = 1
        NameMon = "Dragon Crew Warrior"
        CFrameQuest = CFrame.new(5832.83594, 51.6806107, -1101.51563)
        CFrameMon = CFrame.new(6241.9951171875, 51.522083282471, -1243.9771728516)
    elseif MyLevel >= 1600 and MyLevel <= 1624 then
        Ms = "Dragon Crew Archer [Lv. 1600]"
        QuestName = "AmazonQuest"
        QuestNumber = 2
        NameMon = "Dragon Crew Archer"
        CFrameQuest = CFrame.new(5832.83594, 51.6806107, -1101.51563)
        CFrameMon = CFrame.new(6488.9155273438, 383.38375854492, -110.66246032715)
    elseif MyLevel >= 1625 and MyLevel <= 1649 then
        Ms = "Female Islander [Lv. 1625]"
        QuestName = "AmazonQuest2"
        QuestNumber = 1
        NameMon = "Female Islander"
        CFrameQuest = CFrame.new(5448.86133, 601.516174, 751.130676)
        CFrameMon = CFrame.new(5825.2241210938, 682.89245605469, 704.57958984375)
    elseif MyLevel >= 1650 and MyLevel <= 1699 then
        Ms = "Giant Islander [Lv. 1650]"
        QuestName = "AmazonQuest2"
        QuestNumber = 2
        NameMon = "Giant Islander"
        CFrameQuest = CFrame.new(5448.86133, 601.516174, 751.130676)
        CFrameMon = CFrame.new(4530.3540039063, 656.75695800781, -131.60952758789)
    elseif MyLevel >= 1700 and MyLevel <= 1724 then
        Ms = "Marine Commodore [Lv. 1700]"
        QuestName = "MarineTreeIsland"
        QuestNumber = 1
        NameMon = "Marine Commodore"
        CFrameQuest = CFrame.new(2180.54126, 27.8156815, -6741.5498)
        CFrameMon = CFrame.new(2490.0844726563, 190.4232635498, -7160.0502929688)
    elseif MyLevel >= 1725 and MyLevel <= 1774 then
        Ms = "Marine Rear Admiral [Lv. 1725]"
        QuestName = "MarineTreeIsland"
        QuestNumber = 2
        NameMon = "Marine Rear Admiral"
        CFrameQuest = CFrame.new(2180.54126, 27.8156815, -6741.5498)
        CFrameMon = CFrame.new(3951.3903808594, 229.11549377441, -6912.81640625)
    elseif MyLevel >= 1775 and MyLevel <= 1799 then
        Ms = "Fishman Raider [Lv. 1775]"
        QuestName = "DeepForestIsland3"
        QuestNumber = 1
        NameMon = "Fishman Raider"
        CFrameQuest = CFrame.new(-10581.6563, 330.872955, -8761.18652)
        CFrameMon = CFrame.new(-10322.400390625, 390.94473266602, -8580.0908203125)
    elseif MyLevel >= 1800 and MyLevel <= 1824 then
        Ms = "Fishman Captain [Lv. 1800]"
        QuestName = "DeepForestIsland3"
        QuestNumber = 2
        NameMon = "Fishman Captain"
        CFrameQuest = CFrame.new(-10581.6563, 330.872955, -8761.18652)
        CFrameMon = CFrame.new(-11194.541992188, 442.02795410156, -8608.806640625)
    elseif MyLevel >= 1825 and MyLevel <= 1849 then
        Ms = "Forest Pirate [Lv. 1825]"
        QuestName = "DeepForestIsland"
        QuestNumber = 1
        NameMon = "Forest Pirate"
        CFrameQuest = CFrame.new(-13234.04, 331.488495, -7625.40137)
        CFrameMon = CFrame.new(-13225.809570313, 428.19387817383, -7753.1245117188)
    elseif MyLevel >= 1850 and MyLevel <= 1899 then
        Ms = "Mythological Pirate [Lv. 1850]"
        QuestName = "DeepForestIsland"
        QuestNumber = 2
        NameMon = "Mythological Pirate"
        CFrameQuest = CFrame.new(-13234.04, 331.488495, -7625.40137)
        CFrameMon = CFrame.new(-13869.172851563, 564.95251464844, -7084.4135742188)
    elseif MyLevel >= 1900 and MyLevel <= 1924 then
        Ms = "Jungle Pirate [Lv. 1900]"
        QuestName = "DeepForestIsland2"
        QuestNumber = 1
        NameMon = "Jungle Pirate"
        CFrameQuest = CFrame.new(-12680.3818, 389.971039, -9902.01953)
        CFrameMon = CFrame.new(-11982.221679688, 376.32522583008, -10451.415039063)
    elseif MyLevel >= 1925 and MyLevel <= 1974 then
        Ms = "Musketeer Pirate [Lv. 1925]"
        QuestName = "DeepForestIsland2"
        QuestNumber = 2
        NameMon = "Musketeer Pirate"
        CFrameQuest = CFrame.new(-12680.3818, 389.971039, -9902.01953)
        CFrameMon = CFrame.new(-13282.3046875, 496.23684692383, -9565.150390625)
    elseif MyLevel >= 1975 and MyLevel <= 1999 then
        Ms = "Reborn Skeleton [Lv. 1975]"
        QuestName = "HauntedQuest1"
        QuestNumber = 1
        NameMon = "Reborn Skeleton"
        CFrameQuest = CFrame.new(-9480.8271484375, 142.13066101074, 5566.0712890625)
        CFrameMon = CFrame.new(-8817.880859375, 191.16761779785, 6298.6557617188)
    elseif MyLevel >= 2000 and MyLevel <= 2024 then
        Ms = "Living Zombie [Lv. 2000]"
        QuestName = "HauntedQuest1"
        QuestNumber = 2
        NameMon = "Living Zombie"
        CFrameQuest = CFrame.new(-9480.8271484375, 142.13066101074, 5566.0712890625)
        CFrameMon = CFrame.new(-10125.234375, 183.94705200195, 6242.013671875)
    elseif MyLevel >= 2025 and MyLevel <= 2049 then
        Ms = "Demonic Soul [Lv. 2025]"
        QuestName = "HauntedQuest2"
        QuestNumber = 1
        NameMon = "Demonic Soul"
        CFrameQuest = CFrame.new(-9516.9931640625, 178.00651550293, 6078.4653320313)
        CFrameMon = CFrame.new(-9712.03125, 204.69589233398, 6193.322265625)
    elseif MyLevel >= 2050 and MyLevel <= 2074 then
        Ms = "Posessed Mummy [Lv. 2050]"
        QuestName = "HauntedQuest2"
        QuestNumber = 2
        NameMon = "Posessed Mummy"
        CFrameQuest = CFrame.new(-9516.9931640625, 178.00651550293, 6078.4653320313)
        CFrameMon = CFrame.new(-9545.7763671875, 69.619895935059, 6339.5615234375)    
    elseif MyLevel >= 2075 and MyLevel <= 2099 then
        Ms = "Peanut Scout [Lv. 2075]"
        QuestName = "NutsIslandQuest"
        QuestNumber = 1
        NameMon = "Peanut Scout"
        CFrameQuest = CFrame.new(-2104.35669, 38.1299706, -10194.0654, 0.777809024, -4.20693302e-09, 0.62850064, 1.93921803e-08, 1, -1.73054406e-08, -0.62850064, 2.56483261e-08, 0.777809024)
        CFrameMon = CFrame.new(-2126.40723, 90.5567474, -10301.9639, -0.835617959, 5.5450208e-08, -0.549311042, -1.3585427e-08, 1, 1.21611308e-07, 0.549311042, 1.09083217e-07, -0.835617959)    
    elseif MyLevel >= 2100 and MyLevel <= 2124 then
        Ms = "Peanut President [Lv. 2100]"
        QuestName = "NutsIslandQuest"
        QuestNumber = 2
        NameMon = "Peanut President"
        CFrameQuest = CFrame.new(-2104.35669, 38.1299706, -10194.0654, 0.777809024, -4.20693302e-09, 0.62850064, 1.93921803e-08, 1, -1.73054406e-08, -0.62850064, 2.56483261e-08, 0.777809024)
        CFrameMon = CFrame.new(-2118.75439, 70.3045197, -10509.3223, 0.585819364, 1.20945716e-08, -0.810441673, 7.93158179e-08, 1, 7.225605e-08, 0.810441673, -1.06609832e-07, 0.585819364)    
    elseif MyLevel >= 2125 and MyLevel <= 2149 then
        Ms = "Ice Cream Chef [Lv. 2125]"
        QuestName = "IceCreamIslandQuest"
        QuestNumber = 1
        NameMon = "Ice Cream Chef"
        CFrameQuest = CFrame.new(-820.218994, 65.8453293, -10966.1689, 0.802985847, 8.21155055e-08, -0.595998108, -5.4771629e-08, 1, 6.39845297e-08, 0.595998108, -1.87348856e-08, 0.802985847)
        CFrameMon = CFrame.new(-685.287781, 96.3186417, -10957.5898, -0.859360993, -6.76117935e-08, 0.511369407, -7.04737957e-08, 1, 1.37852645e-08, -0.511369407, -2.41916265e-08, -0.859360993)    
    elseif MyLevel >= 2150 then
        Ms = "Ice Cream Commander [Lv. 2150]"
        QuestName = "IceCreamIslandQuest"
        QuestNumber = 2
        NameMon = "Ice Cream Commander"
        CFrameQuest = CFrame.new(-820.218994, 65.8453293, -10966.1689, 0.802985847, 8.21155055e-08, -0.595998108, -5.4771629e-08, 1, 6.39845297e-08, 0.595998108, -1.87348856e-08, 0.802985847)
        CFrameMon = CFrame.new(-635.736145, 143.049561, -11335.2236, -0.901281416, 2.6901164e-08, 0.433234096, -1.9257731e-09, 1, -6.61001209e-08, -0.433234096, -6.04091213e-08, -0.901281416)    
    end
end
end

CheckLevel()
function EquipWeapon(ToolSe)
if game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe) then
    local tool = game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe)
    wait(.4)
    game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
end
end

section1:addToggle("Auto Farm", _G.AutoFarm, function(v)
_G.AutoFarm = v
_G.FastAttack = v
_G.Main = v 
end)


Wapon = {}
for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do  
    if v:IsA("Tool") then
        table.insert(Wapon ,v.Name)
    end
end
for i,v in pairs(game.Players.LocalPlayer.Character:GetChildren()) do  
    if v:IsA("Tool") then
        table.insert(Wapon, v.Name)
    end
end

local SelectWeapon = section1:addDropdown("Select Weapon", Wapon, function(v)
    _G.SelectWeapon = v
    _G.SelectToolWeaponOld = v
end)

section1:addButton("Refresh Weapon", function()
    SelectWeapon:Clear()
    for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do  
        if v:IsA("Tool") then
            SelectWeapon:Add(v.Name)
        end
    end
    for i,v in pairs(game.Players.LocalPlayer.Character:GetChildren()) do  
        if v:IsA("Tool") then
            SelectWeapon:Add(v.Name)
        end
    end
end) 

function equip()
    pcall(function()
        for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
            if v.Name == _G.SelectWeapon then
                game.Players.LocalPlayer.Character.Humanoid:EquipTool(v)
            end
        end
    end)
end

section1:addToggle("Auto Superhuman", _G.Auto_Superhuman, function(S)
    Superhuman = S
end)

------------------------------------------------------------------- PAGE Stats



local page = venyx:addPage("Stats", 5012544693)
local section2 = page:addSection("Auto Stats")


section2:addToggle("Melee", _G.Melee, function(v)
   _G.Melee = v    
end)


section2:addToggle("Defense", _G.Defense, function(v)
    _G.Defense = v    
end)


section2:addToggle("Sword", _G.Sword, function(v)
   _G.Sword = v
end)


section2:addToggle("Gun", _G.Gun, function(v)
   _G.Gun = v
end)


section2:addToggle("Devil Fruit", _G.Fruit, function(v)
   _G.Fruit = v
end)

PointStats = 1
section2:addSlider("Point", 1, 1, 100, PointStats, function(v)
   PointStats = v
end)

-------------------------------------------------------- PAGE Teleport

local page = venyx:addPage("Teleport", 5012544693)
local section1 = page:addSection("Teleport !")


function TP(P1)
    Distance = (P1.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
    if Distance < 250 then
        Speed = 600
    elseif Distance < 500 then
        Speed = 400
    elseif Distance < 1000 then
        Speed = 350
    elseif Distance >= 1000 then
        Speed = 200
    end
    game:GetService("TweenService"):Create(
        game.Players.LocalPlayer.Character.HumanoidRootPart,
        TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear),
        {CFrame = P1}
    ):Play()
end

function TP2(P1)
	Distance = (P1.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
	if Distance < 1000 then
		Speed = 400
	elseif Distance >= 1000 then
		Speed = 250
	end
    game:GetService("TweenService"):Create(
        game.Players.LocalPlayer.Character.HumanoidRootPart,
        TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear),
        {CFrame = P1}
    ):Play()
    Clip = true
    wait(Distance/Speed)
    Clip = false
end

---------------------- TELEPORT CFRAME
if First_Sea then

section1:addButton("Stop Tween", _G.StopTween, function(S)
    _G.StopTween = S
end)

section1:addButton("Midle Town", function()
    TP2(CFrame.new(-655.97088623047, 7.878026008606, 1573.7612304688))
end)

section1:addButton("Wild Mill", function()
    TP2(CFrame.new(1042.1501464844, 16.299360275269, 1444.3442382813))
end)

section1:addButton("Jungle", function()
    TP2(CFrame.new(-1337.4604492188, 11.852861404419, 497.52340698242))
end)

section1:addButton("Pirate", function()
    TP2(CFrame.new(-1163.3889160156, 44.777843475342, 3842.8276367188))
end)

section1:addButton("Desert", function()
    TP2(CFrame.new(954.02056884766, 6.6275520324707, 4262.611328125))
end)

section1:addButton("Frozen Village", function()
    TP2(CFrame.new(1144.5270996094, 7.3292083740234, -1164.7322998047))
end)

section1:addButton("Colosseum", function()
    TP2(CFrame.new(-1667.5869140625, 39.385631561279, -3135.5817871094))
end)

section1:addButton("Prison", function()
    TP2(CFrame.new(4857.6982421875, 5.6780304908752, 732.75750732422))
end)

section1:addButton("Mob Leader", function()
    TP2(CFrame.new(-2841.9604492188, 7.3560485839844, 5318.1040039063))
end)

section1:addButton("Magma Village", function()
    TP2(CFrame.new(-5328.8740234375, 8.6164798736572, 8427.3994140625))
end)

section1:addButton("UnderWater Gate", function()
    TP2(CFrame.new(3893.953125, 5.3989524841309, -1893.4851074219))
end)

section1:addButton("UnderWater City", function()
    TP2(CFrame.new(61191.12109375, 18.497436523438, 1561.8873291016))
end)

section1:addButton("Fountain City", function()
    TP2(CFrame.new(5244.7133789063, 38.526943206787, 4073.4987792969))
end)

section1:addButton("Sky 1st", function()
    TP2(CFrame.new(-4878.0415039063, 717.71246337891, -2637.7294921875))
end)

section1:addButton("Sky 2nd", function()
    TP2(CFrame.new(-7899.6157226563, 5545.6030273438, -422.21798706055))
end)

section1:addButton("Sky 3rd", function()
   TP2(CFrame.new(-7868.5288085938, 5638.205078125, -1482.5548095703))
end)
end

if Second_Sea then

section1:addButton("Dock",function()
    TP2(CFrame.new(82.9490662, 18.0710983, 2834.98779))
end)

section1:addButton("Flamingo Room",function()
    TP2(CFrame.new(2302.19019, 15.1778421, 663.811035))
end)

section1:addButton("Mansion",function()
    TP2(CFrame.new(-390.096313, 331.886475, 673.464966))
end)

section1:addButton("Cafe",function()
    TP2(CFrame.new(-385.250916, 73.0458984, 297.388397))
end)

section1:addButton("Green Zone",function()
    TP2(CFrame.new(-2372.14697, 72.9919434, -3166.51416))
end)

section1:addButton("Kingdom of Rose",function()
    TP2(CFrame.new(-394.983521, 118.503128, 1245.8446))
end)

section1:addButton("Factroy",function()
    TP2(CFrame.new(430.42569, 210.019623, -432.504791))
end)

section1:addButton("Big Colosseum",function()
    TP2(CFrame.new(-1836.58191, 44.5890656, 1360.30652))
end)

section1:addButton("GraveIsland",function()
    TP2(CFrame.new(-5411.47607, 48.8234024, -721.272522))
end)

section1:addButton("Snow Mountain",function()
    TP2(CFrame.new(511.825226, 401.765198, -5380.396))
end)

section1:addButton("Cold Island",function()
    TP2(CFrame.new(-6026.96484, 14.7461271, -5071.96338))
end)

section1:addButton("Hot Island",function()
    TP2(CFrame.new(-5478.39209, 15.9775667, -5246.9126))
end)

section1:addButton("Cursed Ship",function()
    TP2(CFrame.new(902.059143, 124.752518, 33071.8125))
end)

section1:addButton("IceCastle",function()
    TP2(CFrame.new(5400.40381, 28.21698, -6236.99219))
end)

section1:addButton("Forgotten Island",function()
    TP2(CFrame.new(-3043.31543, 238.881271, -10191.5791))
end)

section1:addButton("Usoapp Island",function()
    TP2(CFrame.new(4748.78857, 8.35370827, 2849.57959))
end)
end

if Third_Sea then

section1:addButton("Port Towen",function()
    TP2(CFrame.new(-610.309692, 57.8323097, 6436.33594))
end)
section1:addButton("Hydra Island",function()
    TP2(CFrame.new(5229.99561, 603.916565, 345.154022))
end)
section1:addButton("Great Tree",function()
    TP2(CFrame.new(2174.94873, 28.7312393, -6728.83154))
end)
section1:addButton("Castle on the Sea",function()
    TP2(CFrame.new(-5477.62842, 313.794739, -2808.4585))
end)
section1:addButton("Floating Turtle",function()
    TP2(CFrame.new(-10919.2998, 331.788452, -8637.57227))
end)
section1:addButton("Mansion",function()
    TP2(CFrame.new(-12553.8125, 332.403961, -7621.91748))
end)
section1:addButton("Secret Temple",function()
    TP2(CFrame.new(5217.35693, 6.56511116, 1100.88159))
end)
section1:addButton("Friendly Arena",function()
    TP2(CFrame.new(5220.28955, 72.8193436, -1450.86304))
end)
section1:addButton("Beautiful Pirate Domain",function()
    TP2(CFrame.new(5310.8095703125, 21.594484329224, 129.39053344727))
end)
section1:addButton("Teler Park",function()
    TP2(CFrame.new(-9512.3623046875, 142.13258361816, 5548.845703125))
end)
section1:addButton("Peanut Island",function()
    TP2(CFrame.new(-2062.67773, 38.1294556, -10287.752, -0.258864403, 0, -0.965913653, 0, 1, 0, 0.965913653, 0, -0.258864403))
end)
section1:addButton("Ice Cream Island",function()
    TP2(CFrame.new(-840.188477, 65.8452759, -10877.3789, -0.573598981, 0, 0.819136262, 0, 1, 0, -0.819136262, 0, -0.573598981))
end)
end

-------------------------------------------------------------------- PAGE MISC


local page = venyx:addPage("Misc", 5012544693)
local section1 = page:addSection("Server")

section1:addButton("Server hop", function()
    local PlaceID = game.PlaceId
        local AllIDs = {}
        local foundAnything = ""
        local actualHour = os.date("!*t").hour
        local Deleted = false
        local File =
            pcall(
            function()
                AllIDs = game:GetService("HttpService"):JSONDecode(readfile("NotSameServers.json"))
            end
        )
        if not File then
            table.insert(AllIDs, actualHour)
            writefile("NotSameServers.json", game:GetService("HttpService"):JSONEncode(AllIDs))
        end
        function TPReturner()
            local Site
            if foundAnything == "" then
                Site =
                    game.HttpService:JSONDecode(
                    game:HttpGet(
                        "https://games.roblox.com/v1/games/" .. PlaceID .. "/servers/Public?sortOrder=Asc&limit=100"
                    )
                )
            else
                Site =
                    game.HttpService:JSONDecode(
                    game:HttpGet(
                        "https://games.roblox.com/v1/games/" ..
                            PlaceID .. "/servers/Public?sortOrder=Asc&limit=100&cursor=" .. foundAnything
                    )
                )
            end
            local ID = ""
            if Site.nextPageCursor and Site.nextPageCursor ~= "null" and Site.nextPageCursor ~= nil then
                foundAnything = Site.nextPageCursor
            end
            local num = 0
            for i, v in pairs(Site.data) do
                local Possible = true
                ID = tostring(v.id)
                if tonumber(v.maxPlayers) > tonumber(v.playing) then
                    for _, Existing in pairs(AllIDs) do
                        if num ~= 0 then
                            if ID == tostring(Existing) then
                                Possible = false
                            end
                        else
                            if tonumber(actualHour) ~= tonumber(Existing) then
                                local delFile =
                                    pcall(
                                    function()
                                        delfile("NotSameServers.json")
                                        AllIDs = {}
                                        table.insert(AllIDs, actualHour)
                                    end
                                )
                            end
                        end
                        num = num + 1
                    end
                    if Possible == true then
                        table.insert(AllIDs, ID)
                        wait()
                        pcall(
                            function()
                                writefile("NotSameServers.json", game:GetService("HttpService"):JSONEncode(AllIDs))
                                wait()
                                game:GetService("TeleportService"):TeleportToPlaceInstance(
                                    PlaceID,
                                    ID,
                                    game.Players.LocalPlayer
                                )
                            end
                        )
                        wait(4)
                    end
                end
            end
        end

        function Teleport()
            while wait() do
                pcall(
                    function()
                        TPReturner()
                        if foundAnything ~= "" then
                            TPReturner()
                        end
                    end
                )
            end
        end

        Teleport()
end)

section1:addButton("Rejoin", function()
	game:GetService("TeleportService"):Teleport(game.PlaceId, game:GetService("Players").localPlayer)
end)

section1:addButton("Fps Boost", function(P)
    local decalsyeeted = true
    local g = game
    local w = g.Workspace
    local l = g.Lighting
    local t = w.Terrain
    t.WaterWaveSize = 0
    t.WaterWaveSpeed = 0
    t.WaterReflectance = 0
    t.WaterTransparency = 0
    l.GlobalShadows = false
    l.FogEnd = 9e9
    l.Brightness = 0
    settings().Rendering.QualityLevel = "Level01"
    for i, v in pairs(g:GetDescendants()) do
        if v:IsA("Part") or v:IsA("Union") or v:IsA("CornerWedgePart") or v:IsA("TrussPart") then 
            v.Material = "Plastic"
            v.Reflectance = 0
        elseif v:IsA("Decal") or v:IsA("Texture") and decalsyeeted then
            v.Transparency = 1
        elseif v:IsA("ParticleEmitter") or v:IsA("Trail") then
            v.Lifetime = NumberRange.new(0)
        elseif v:IsA("Explosion") then
            v.BlastPressure = 1
            v.BlastRadius = 1
        elseif v:IsA("Fire") or v:IsA("SpotLight") or v:IsA("Smoke") or v:IsA("Sparkles") then
            v.Enabled = false
        elseif v:IsA("MeshPart") then
            v.Material = "Plastic"
            v.Reflectance = 0
            v.TextureID = 10385902758728957
        end
    end
    for i, e in pairs(l:GetChildren()) do
        if e:IsA("BlurEffect") or e:IsA("SunRaysEffect") or e:IsA("ColorCorrectionEffect") or e:IsA("BloomEffect") or e:IsA("DepthOfFieldEffect") then
            e.Enabled = false
        end
    end
end)

local section2 = page:addSection("Team")

section2:addButton("Pirate", function()
    local args = {
        [1] = "SetTeam",
        [2] = "Pirates"
    }
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args)) 
    local args = {
        [1] = "BartiloQuestProgress"
    }
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)

section2:addButton("Marine", function()
    local args = {
        [1] = "SetTeam",
        [2] = "Marines"
    }
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    local args = {
        [1] = "BartiloQuestProgress"
    }
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
-------------------------------------------------------------------------- PAGE Setting

local page = venyx:addPage("Setting", 5012544693)
local section1 = page:addSection("Setting and Others")

section1:addToggle("Fast Attack", true, function(F)
    _G.FastAttack = F
end)

section1:addToggle("AutoHaki", true, function(h)
   Auto_Haki = h 
end)
function AutoHaki()
    if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
        local args = {
            [1] = "Buso"
        }
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end
end
Auto_Haki = true
spawn(function()
    while wait(.1) do
        if Auto_Haki then
            if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Buso")
            end
        end
    end
end)


section1:addToggle("Auto Quest", true, function(v)
AutoQuest = v
end)

section1:addKeybind("Toggle Keybind", Enum.KeyCode.RightControl, function()
    print("Activated Keybind")
    venyx:toggle()
    end, function()
    print("Changed Keybind")
    end)
    
section1:addButton("ResetCharacter", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart:Destroy()
end)

section1:addButton("Right Destroy", function()
    game.Players.LocalPlayer.Character.RightUpperLeg:Destroy()
end)

section1:addButton("Left Destroy", function()
    game.Players.LocalPlayer.Character.LeftUpperLeg:Destroy()
end)






spawn(function()
    while wait() do
        if _G.AutoFarm then
            autofarm()
        end
    end
end)
game:GetService("RunService").Heartbeat:Connect(
function()
    if _G.AutoFarm then
        if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Humanoid") then
    end
end
end)

local LocalPlayer = game:GetService("Players").LocalPlayer
local VirtualUser = game:GetService('VirtualUser')

function totarget(CFgo)
local tween_s = game:service"TweenService"
local info = TweenInfo.new((game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart.Position - CFgo.Position).Magnitude/300, Enum.EasingStyle.Linear)
local tween, err = pcall(function()
    tween = tween_s:Create(game.Players.LocalPlayer.Character["HumanoidRootPart"], info, {CFrame = CFgo})
    tween:Play()
end)
if not tween then return err end
end

function StopTween()
pcall(function()
    tween:Cancel()
    _G.StopTween = true
    wait()
    _G.StopTween = false
end)
end

AutoQuest = true
function autofarm()
if _G.AutoFarm then
    if AutoQuest then
        if LocalPlayer.PlayerGui.Main.Quest.Visible == false then
            _G.FastAttack = false
            StopTween()
            StatrMagnet = false
            CheckLevel()
            repeat totarget(CFrameQuest) wait() until _G.StopTween == true or not _G.AutoFarm or (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - CFrameQuest.Position).Magnitude <= 20
            wait(0.9)
            if _G.AutoFarm then
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("SetSpawnPoint")
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", QuestName, QuestNumber)
            end
        elseif game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
            _G.FastAttack = true
            CheckLevel()
            if game:GetService("Workspace").Enemies:FindFirstChild(Ms) then
                pcall(
                    function()
                        for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                            CheckLevel()  
                            if v.Name == Ms then
                                repeat wait()
                                    spawn(function()
                                        if game:GetService("Workspace").Enemies:FindFirstChild(Ms) and v.Humanoid.Health > 0 and v:FindFirstChild("Humanoid") then
                                            if LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text:find(NameMon) then
                                                EquipWeapon(_G.SelectWeapon)
                                                totarget(v.HumanoidRootPart.CFrame * CFrame.new(0,40,0))
                                                v.Humanoid.PlatformStand = true
                                                v.Humanoid.Sit = true
                                                v.HumanoidRootPart.CanCollide = false
                                                v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
                                                ToMob = v.HumanoidRootPart.CFrame
                                                StatrMagnet = true
                                            else
                                                StopTween()
                                                local args = {
                                                    [1] = "AbandonQuest"
                                                 }
                                                 game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
                                            end  
                                        else
                                            CheckLevel() 
                                            StatrMagnet = false
                                            totarget(CFrameMon)
                                        end 
                                    end)
                                until not v.Parent or v.Humanoid.Health <= 0 or _G.AutoFarm == false or LocalPlayer.PlayerGui.Main.Quest.Visible == false
                                CheckLevel() 
                                StatrMagnet = false
                            end
                        end
                    end
                )
            else
                CheckLevel()
                StatrMagnet = false
                totarget(CFrameMon)
            end 
        end
    end
end
end

spawn(function()
    pcall(function()
       game:GetService("RunService").Heartbeat:Connect(function()
        if _G.AutoFarm then
          if not game:GetService("Workspace"):FindFirstChild("LOL") then
             local Paertaiteen = Instance.new("Part")
             Paertaiteen.Name = "LOL"
             Paertaiteen.Parent = game.Workspace
             Paertaiteen.Anchored = true
             Paertaiteen.Transparency = 1
             Paertaiteen.Size = Vector3.new(30,0.5,30)
             Paertaiteen.Material = "Neon"
             while true do 
                 wait(0.1) 
                 game:GetService('TweenService'):Create(
                     Paertaiteen,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.InOut),
                 {Color = Color3.fromRGB(255, 0, 0)}):Play() 
                 wait(.5)
 
                 game:GetService('TweenService'):Create(
                     Paertaiteen,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.InOut),
                 {Color = Color3.fromRGB(255, 155, 0)}):Play() 
                 wait(.5)
 
                 game:GetService('TweenService'):Create(
                     Paertaiteen,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.InOut),
                 {Color = Color3.fromRGB(255, 255, 0)}):Play() 
                 wait(.5)
 
                 game:GetService('TweenService'):Create(
                     Paertaiteen,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.InOut),
                 {Color = Color3.fromRGB(0, 255, 0)}):Play() 
                 wait(.5)
 
                 game:GetService('TweenService'):Create(
                     Paertaiteen,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.InOut),
                 {Color = Color3.fromRGB(0, 255, 255)}):Play() 
                 wait(.5)
 
                 game:GetService('TweenService'):Create(
                     Paertaiteen,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.InOut),
                 {Color = Color3.fromRGB(0, 155, 255)}):Play() 
                 wait(.5)
 
                 game:GetService('TweenService'):Create(
                     Paertaiteen,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.InOut),
                 {Color = Color3.fromRGB(255, 0, 255)}):Play() 
                 wait(.5)
 
                 game:GetService('TweenService'):Create(
                     Paertaiteen,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.InOut),
                 {Color = Color3.fromRGB(255, 0, 155)}):Play() 
                 wait(.5)
             end 
         elseif game:GetService("Workspace"):FindFirstChild("LOL") then
             game.Workspace["LOL"].CFrame = CFrame.new(game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame.X,game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame.Y - 3.92,game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame.Z)
         end
     else
         if game:GetService("Workspace"):FindFirstChild("LOL") then
             game:GetService("Workspace"):FindFirstChild("LOL"):Destroy()
         end
        end
    end)
 end)
end)

spawn(function()
	pcall(function()
		while wait(.1) do
			if AutoSetSpawn and game.Players.LocalPlayer.Character.Humanoid.Health > 0 then
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("SetSpawnPoint")
			end
		end
	end)
end)
 
spawn(function()
while wait() do
if _G.EquipMelee then
    pcall(function()
        for i,v in pairs(game:GetService("Players").LocalPlayer.Backpack:GetChildren()) do
           if v.ToolTip == "Melee" then
          if game.Players.LocalPlayer.Backpack:FindFirstChild(tostring(v.Name)) then
              local ToolSe = tostring(v.Name)
             local tool = game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe)
             wait(.4)
             game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
          end
           end
        end
    end)
end
end
end)

spawn(function()
    while wait() do
        pcall(function()
            if _G.AutoNew == true then
                if _G.SelectWeapon == nil then
                    _G.EquipMelee  = true
                end
            else 
                _G.EquipMelee = false
            end
        end)
    end
end)

local CombatFrameworkR = require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework) 

local VirtualUser = game:GetService('VirtualUser')

local CameraShakerR = require(game.ReplicatedStorage.Util.CameraShaker)
_G.FastAttack = true
spawn(function()
    game:GetService('RunService').Heartbeat:connect(function()
        if _G.FastAttack then
            pcall(function()
                CombatFrameworkR.activeController.attacking = false
                CombatFrameworkR.activeController.blocking = false
                CombatFrameworkR.activeController.timeToNextAttack = tick() -1
                CombatFrameworkR.activeController.timeToNextBlock = 0
                CombatFrameworkR.activeController.increment = 3
                CombatFrameworkR.activeController.hitboxMagnitude = 120
                game.Players.LocalPlayer.Character.Stun.Value = 0
                game.Players.LocalPlayer.Character.Humanoid.Sit = false
                VirtualUser:CaptureController()
                VirtualUser:Button1Down(Vector2.new(1280, 672))
                CameraShakerR:Stop()
            end)
        end
    end)
end)

spawn(function()
    for i = 1,math,9999999999999999999999999999999999999999 do game:GetService('RunService').Heartbeat:wait()
        if _G.FastAttack then
        VirtualUser:CaptureController()
        VirtualUser:Button1Down(Vector2.new(1280, 672))
    end
end
end)




function bring2()
    local plr = game.Players.LocalPlayer
    pcall(function()
        sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
    end)
end
spawn(function()
    while wait(.1) do
        if _G.AutoFarm then
            bring2()
        end
    end
end)

spawn(function()
    while true do
        pcall(function()
            if _G.AutoFarm and StatrMagnet then
                CheckLevel()
                for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
                    if v.Name == Ms and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
                        if syn then
                            if isnetworkowner(v.HumanoidRootPart) then
                                if v.Name == "Monkey [Lv. 14]" or v.Name == "Factory Staff [Lv. 800]" or v.Name == "Dragon Crew Warrior [Lv. 1575]" or v.Name == "Dragon Crew Archer [Lv. 1600]" and (v.HumanoidRootPart.Position-game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 200 then
                                    if HideHitBlox then
                                        v.HumanoidRootPart.Transparency = 1
                                    else
                                        v.HumanoidRootPart.Transparency = 70
                                    end
                                    v.Humanoid.PlatformStand = true
                                    v.Humanoid.Sit = true
                                    v.HumanoidRootPart.CanCollide = false
                                    v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
                                    v.HumanoidRootPart.CFrame = ToMob
                                elseif v.Name == Ms and (v.HumanoidRootPart.Position-game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 400 then
                                    if HideHitBlox then
                                        v.HumanoidRootPart.Transparency = 1
                                    else
                                        v.HumanoidRootPart.Transparency = 70
                                    end
                                    v.Humanoid.PlatformStand = true
                                    v.Humanoid.Sit = true
                                    v.HumanoidRootPart.CanCollide = false
                                    v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
                                    v.HumanoidRootPart.CFrame = ToMob
                                end
                            end
                        else
                            if v.Name == "Monkey [Lv. 14]" or v.Name == "Factory Staff [Lv. 800]" or v.Name == "Dragon Crew Warrior [Lv. 1575]" or v.Name == "Dragon Crew Archer [Lv. 1600]" and (v.HumanoidRootPart.Position-game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 200 then
                                if HideHitBlox then
                                    v.HumanoidRootPart.Transparency = 1
                                else
                                    v.HumanoidRootPart.Transparency = 70
                                end
                                v.Humanoid.PlatformStand = true
                                v.Humanoid.Sit = true
                                v.HumanoidRootPart.CanCollide = false
                                v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
                                v.HumanoidRootPart.CFrame = ToMob
                            elseif v.Name == Ms and (v.HumanoidRootPart.Position-game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 400 then
                                if HideHitBlox then
                                    v.HumanoidRootPart.Transparency = 1
                                else
                                    v.HumanoidRootPart.Transparency = 70
                                end
                                v.Humanoid.PlatformStand = true
                                v.Humanoid.Sit = true
                                v.HumanoidRootPart.CanCollide = false
                                v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
                                v.HumanoidRootPart.CFrame = ToMob
                            end
                        end
                    end
                end
            end 
        end)
        wait()
    end
end)


if _G.FPSBoost then
    spawn(function()
        wait(3)
        local decalsyeeted = true
        local g = game
        local w = g.Workspace
        local l = g.Lighting
        local t = w.Terrain
        t.WaterWaveSize = 0
        t.WaterWaveSpeed = 0
        t.WaterReflectance = 0
        t.WaterTransparency = 0
        l.GlobalShadows = false
        l.FogEnd = 9e9
        l.Brightness = 0
        settings().Rendering.QualityLevel = "Level01"
        for i, v in pairs(g:GetDescendants()) do
            if v:IsA("Part") or v:IsA("Union") or v:IsA("CornerWedgePart") or v:IsA("TrussPart") then 
                v.Material = "Plastic"
                v.Reflectance = 0
            elseif v:IsA("Decal") or v:IsA("Texture") and decalsyeeted then
                v.Transparency = 1
            elseif v:IsA("ParticleEmitter") or v:IsA("Trail") then
                v.Lifetime = NumberRange.new(0)
            elseif v:IsA("Explosion") then
                v.BlastPressure = 1
                v.BlastRadius = 1
            elseif v:IsA("Fire") or v:IsA("SpotLight") or v:IsA("Smoke") or v:IsA("Sparkles") then
                v.Enabled = false
            elseif v:IsA("MeshPart") then
                v.Material = "Plastic"
                v.Reflectance = 0
                v.TextureID = 10385902758728957
            end
        end
        for i, e in pairs(l:GetChildren()) do
            if e:IsA("BlurEffect") or e:IsA("SunRaysEffect") or e:IsA("ColorCorrectionEffect") or e:IsA("BloomEffect") or e:IsA("DepthOfFieldEffect") then
                e.Enabled = false
            end
        end
    end)
end

spawn(function()
    while wait() do
        if game.Players.localPlayer.Data.Points.Value >= PointStats then
            if _G.Melee then
                local args = {
                    [1] = "AddPoint",
                    [2] = "Melee",
                    [3] = PointStats
                }
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
            end 
            if _G.Defense then
                local args = {
                    [1] = "AddPoint",
                    [2] = "Defense",
                    [3] = PointStats
                }
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
            end 
            if _G.Sword then
                local args = {
                    [1] = "AddPoint",
                    [2] = "Sword",
                    [3] = PointStats
                }
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
            end 
            if _G.Gun then
                local args = {
                    [1] = "AddPoint",
                    [2] = "Gun",
                    [3] = PointStats
                }
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
            end 
            if _G.Fruit then
                local args = {
                    [1] = "AddPoint",
                    [2] = "Demon Fruit",
                    [3] = PointStats
                }
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
            end
        end
    end
 end)

 spawn(function()
	while wait(.1) do
		if _G.AutoStat then
			for i,v in pairs(_G.AutoStat) do
				if v == "Melee" and game.Players.LocalPlayer.Data.Stats.Melee.Level.Value ~= 2100 then
					repeat game:GetService("RunService").Heartbeat:wait()
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AddPoint", "Melee", 1)
					until game.Players.LocalPlayer.Data.Stats.Melee.Level.Value == 2100
				elseif v == "Defense" and game.Players.LocalPlayer.Data.Stats.Defense.Level.Value ~= 2100 then
					repeat game:GetService("RunService").Heartbeat:wait()
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AddPoint", "Defense", 1)
					until game.Players.LocalPlayer.Data.Stats.Defense.Level.Value == 2100
				elseif v == "Sword" and game.Players.LocalPlayer.Data.Stats.Sword.Level.Value ~= 2100 then
					repeat game:GetService("RunService").Heartbeat:wait()
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AddPoint", "Sword", 1)
					until game.Players.LocalPlayer.Data.Stats.Sword.Level.Value == 2100
				elseif v == "Gun" and game.Players.LocalPlayer.Data.Stats.Gun.Level.Value ~= 2100 then
					repeat game:GetService("RunService").Heartbeat:wait()
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AddPoint", "Gun", 1)
					until game.Players.LocalPlayer.Data.Stats.Gun.Level.Value == 2100
				elseif v == "DevilFruit" and game.Players.LocalPlayer.Data.Stats["Demon Fruit"].Level.Value ~= 2100 then
					repeat game:GetService("RunService").Heartbeat:wait()
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AddPoint", "Demon Fruit", 1)
					until game.Players.LocalPlayer.Data.Stats.Gun.Level.Value == 2100
				end
			end
		end
	end
end)

spawn(function()
	pcall(function()
		while wait(.1) do
			if Superhuman or AutoFullySuperhuman then
				if game.Players.LocalPlayer.Backpack:FindFirstChild("Combat") or game.Players.LocalPlayer.Character:FindFirstChild("Combat") or game.Players.LocalPlayer.Backpack:FindFirstChild("Electric Claw") or game.Players.LocalPlayer.Character:FindFirstChild("Electric Claw") or game.Players.LocalPlayer.Backpack:FindFirstChild("Sharkman Karate") or game.Players.LocalPlayer.Character:FindFirstChild("Sharkman Karate") or game.Players.LocalPlayer.Backpack:FindFirstChild("Death Step") or game.Players.LocalPlayer.Character:FindFirstChild("Death Step") then
					local args = {
						[1] = "BuyBlackLeg"
					}
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
				end
				if game.Players.LocalPlayer.Character:FindFirstChild("Combat") or game.Players.LocalPlayer.Backpack:FindFirstChild("Combat") or game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg") or game.Players.LocalPlayer.Character:FindFirstChild("Black Leg") or game.Players.LocalPlayer.Backpack:FindFirstChild("Electro") or game.Players.LocalPlayer.Character:FindFirstChild("Electro") or game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate") or game.Players.LocalPlayer.Character:FindFirstChild("Fishman Karate") or game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw") or game.Players.LocalPlayer.Character:FindFirstChild("Dragon Claw") or game.Players.LocalPlayer.Backpack:FindFirstChild("Superhuman") or game.Players.LocalPlayer.Character:FindFirstChild("Superhuman") then
					if game.Players.LocalPlayer.Backpack:FindFirstChild("Combat") or game.Players.LocalPlayer.Character:FindFirstChild("Combat") then
						SelectToolWeapon = "Combat"
						SelectToolWeaponOld = "Combat"
					end
					if game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg") or game:GetService("Players").LocalPlayer.Character:FindFirstChild("Black Leg") then
						SelectToolWeapon = "Black Leg"
						SelectToolWeaponOld = "Black Leg"
					end
					if game.Players.LocalPlayer.Backpack:FindFirstChild("Electro") or game:GetService("Players").LocalPlayer.Character:FindFirstChild("Electro") then
						SelectToolWeapon = "Electro"
						SelectToolWeaponOld = "Electro"
					end
					if game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate") or game:GetService("Players").LocalPlayer.Character:FindFirstChild("Fishman Karate") then
						SelectToolWeapon = "Fishman Karate"
						SelectToolWeaponOld = "Fishman Karate"
					end
					if game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw") or game:GetService("Players").LocalPlayer.Character:FindFirstChild("Dragon Claw") then
						SelectToolWeapon = "Dragon Claw"
						SelectToolWeaponOld = "Dragon Claw"
					end
					if game.Players.LocalPlayer.Backpack:FindFirstChild("Superhuman") or game:GetService("Players").LocalPlayer.Character:FindFirstChild("Superhuman") then
						SelectToolWeapon = "Superhuman"
						SelectToolWeaponOld = "Superhuman"
					end
					if (game.Players.LocalPlayer.Character:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Character:FindFirstChild("Black Leg").Level.Value >= 300) or (game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg").Level.Value >= 300) then
						local args = {
							[1] = "BuyElectro"
						}
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
					end
					if (game.Players.LocalPlayer.Character:FindFirstChild("Electro") and game.Players.LocalPlayer.Character:FindFirstChild("Electro").Level.Value >= 300) or (game.Players.LocalPlayer.Backpack:FindFirstChild("Electro") and game.Players.LocalPlayer.Backpack:FindFirstChild("Electro").Level.Value >= 300) then
						local args = {
							[1] = "BuyFishmanKarate"
						}
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
					end
					if (game.Players.LocalPlayer.Character:FindFirstChild("Fishman Karate") and game.Players.LocalPlayer.Character:FindFirstChild("Fishman Karate").Level.Value >= 300) or (game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate") and game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate").Level.Value >= 300) then
                        if AutoFullySuperhuman then
                            if game.Players.LocalPlayer.Data.Level.Value >= 1100 then
                                if game.Players.LocalPlayer.Data.Fragments.Value <= 1499 then
                                    RaidSuperhuman = true
                                    _G.SelectRaid = "Flame"
                                    Auto_Farm = false
                                elseif game.Players.LocalPlayer.Data.Fragments.Value >= 1500 then
                                    RaidSuperhuman = false
                                    if _G.AutoFarm and RaidSuperhuman == false then
                                        Auto_Farm = true
                                    end
                                    local args = {
                                        [1] = "BlackbeardReward",
                                        [2] = "DragonClaw",
                                        [3] = "1"
                                    }
                                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
                                    local args = {
                                        [1] = "BlackbeardReward",
                                        [2] = "DragonClaw",
                                        [3] = "2"
                                    }
                                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
                                end
                            end
						elseif not AutoFullySuperhuman then
							local args = {
								[1] = "BlackbeardReward",
								[2] = "DragonClaw",
								[3] = "1"
							}
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
							local args = {
								[1] = "BlackbeardReward",
								[2] = "DragonClaw",
								[3] = "2"
							}
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
						end
					end
					if (game.Players.LocalPlayer.Character:FindFirstChild("Dragon Claw") and game.Players.LocalPlayer.Character:FindFirstChild("Dragon Claw").Level.Value >= 300) or (game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw") and game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw").Level.Value >= 300) then
						local args = {
							[1] = "BuySuperhuman"
						}
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
					end
				end
			end
		end
	end)
end)


venyx:SelectPage(venyx.pages[1], true)
