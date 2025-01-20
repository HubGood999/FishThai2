



setfpscap(1)
wait(5)
setfpscap(999)



--//---//----//---//---//----//---//---//----//---//---//----//---//---//----//
--// XXX Hub by XXX --//
_G.AntiAFK = true

if not _G.AntiAFK then
    _G.AntiAFK = false -- กำหนดค่าเริ่มต้นให้เป็น false
end

-- สร้างอินสแตนซ์ของ VirtualUser
local VirtualUser = game:GetService("VirtualUser")

task.spawn(function()
    while true do -- ลูปแบบต่อเนื่อง
        task.wait(5) -- หยุดรอสั้นๆ เพื่อหลีกเลี่ยงการแฮงค์

        if _G.AntiAFK then
            -- จำลองการกดปุ่มเมาส์ขวา
            VirtualUser:CaptureController()
            VirtualUser:ClickButton2(Vector2.new())
        end
    end
end)



wait(0.1)
warn("Script : Fish [FREE]")
wait(0.1)
warn("Anti AFK Actived")
wait(0.1)
warn("Thank to " .. game.Players.LocalPlayer.Name)



--//---//----//---//---//----//---//---//----//---//---//----//---//---//----//
--//---//----//---//---//----//---//---//----//---//---//----//---//---//----//
--// AutoLevelFarm--//


_G.index = false -- กำหนดค่าเริ่มต้นให้ _G.index เป็น false
_G.indexV2 = false 
_G.Tool1 = false -- Flag to control the loop
_G.Autoprompt = false


task.spawn(function()
    -- เช็คว่าค่า _G.index เป็น true หรือไม่ ถ้าเป็น true จะเริ่มทำงาน
    while true do
        task.wait(0.1)  -- รอเวลานิดหน่อยก่อนทำงานต่อ
        if _G.index then
           local positions = {
    Vector3.new(2435, 130, -730),
    Vector3.new(2445, 128, -720),
    Vector3.new(2446, 128, -732),
    Vector3.new(2447, 128, -712),
    Vector3.new(2449, 132, -703),
    Vector3.new(2453, 128, -693),
    Vector3.new(2453, 128, -686),
    Vector3.new(2453, 129, -678),
    Vector3.new(2461, 129, -678),
    Vector3.new(2474, 130, -682),
    Vector3.new(2481, 130, -681),
    Vector3.new(2463, 129, -660),
    Vector3.new(2469, 128, -662),
    Vector3.new(2473, 130, -656),
    Vector3.new(2484, 130, -656),
    Vector3.new(2484, 128, -664),
    Vector3.new(2492, 130, -656),
    Vector3.new(2500, 128, -664),
    Vector3.new(2500, 130, -656),
    Vector3.new(2514, 128, -663),
    Vector3.new(2514, 130, -657),
    Vector3.new(2532, 131, -616),
    Vector3.new(2539, 131, -619),
    Vector3.new(2544, 130, -623),
    Vector3.new(2542, 131, -636),
    Vector3.new(2535, 133, -638),
    Vector3.new(2529, 133, -640),
    Vector3.new(2545, 128, -644),
    Vector3.new(2546, 128, -651),
    Vector3.new(2550, 129, -658),
    Vector3.new(2560, 130, -690),
    Vector3.new(2567, 130, -693),
    Vector3.new(2574, 134, -698),
    Vector3.new(2581, 131, -696),
    Vector3.new(2588, 130, -696),
    Vector3.new(2598, 133, -690),
    Vector3.new(2612, 130, -684),
    Vector3.new(2620, 129, -685),
    Vector3.new(2627, 129, -685),
    Vector3.new(2633, 129, -684),
    Vector3.new(2640, 129, -684),
    Vector3.new(2647, 130, -680),
    Vector3.new(2647, 128, -688),
    Vector3.new(2654, 128, -686),
    Vector3.new(2654, 130, -679),
    Vector3.new(2660, 134, -688),
    Vector3.new(2663, 130, -694),
    Vector3.new(2664, 130, -678),
    Vector3.new(2671, 130, -678),
    Vector3.new(2672, 128, -685),
    Vector3.new(2678, 130, -684),
    Vector3.new(2685, 130, -684),
    Vector3.new(2692, 130, -684),
    Vector3.new(2698, 130, -683),
    Vector3.new(2705, 130, -682),
    Vector3.new(2712, 130, -681),
    Vector3.new(2719, 130, -681),
    Vector3.new(2726, 130, -687),
    Vector3.new(2731, 133, -694),
    Vector3.new(2733, 130, -685),
    Vector3.new(2546, 130, -726),
    Vector3.new(2539, 130, -728),
    Vector3.new(2532, 130, -728),
    Vector3.new(2525, 130, -727),
    Vector3.new(2505, 131, -720),
    Vector3.new(2499, 131, -720),
    Vector3.new(2468, 130, -733),
    Vector3.new(2476, 130, -735),
    Vector3.new(2482, 130, -735),
    Vector3.new(2432, 130, -730),
    Vector3.new(2440, 129, -731),
    Vector3.new(2447, 128, -733),
    Vector3.new(2448, 128, -726),
    Vector3.new(2446, 128, -718),
    Vector3.new(2429, 128, -784),
    Vector3.new(2434, 128, -803),
    Vector3.new(2453, 131, -770),
    Vector3.new(2484, 131, -798),
    Vector3.new(2491, 131, -798),
    Vector3.new(2498, 131, -798),
    Vector3.new(2506, 131, -799),
    Vector3.new(2514, 131, -799),
    Vector3.new(2523, 131, -799),
    Vector3.new(2528, 131, -799),
    Vector3.new(2531, 132, -809),
    Vector3.new(2538, 130, -776),
    Vector3.new(2545, 129, -767),
    Vector3.new(2549, 130, -786),
    Vector3.new(2556, 130, -785),
    Vector3.new(2563, 131, -784),
    Vector3.new(2557, 130, -765),
    Vector3.new(2568, 131, -791),
    Vector3.new(2573, 131, -798),
    Vector3.new(2578, 131, -805),
    Vector3.new(2561, 130, -821),
    Vector3.new(2624, 131, -729),
    Vector3.new(2620, 132, -737),
    Vector3.new(2618, 128, -746),
    Vector3.new(2618, 128, -756),
    Vector3.new(2618, 128, -764),
    Vector3.new(2618, 128, -771),
    Vector3.new(2618, 128, -779),
    Vector3.new(2618, 128, -788),
    Vector3.new(2632, 130, -702),
    Vector3.new(2631, 130, -708),
    Vector3.new(2631, 130, -715),
    Vector3.new(2638, 132, -716),
    Vector3.new(2645, 130, -717),
    Vector3.new(2652, 130, -711),
    Vector3.new(2659, 131, -717),
    Vector3.new(2667, 130, -717),
    Vector3.new(2674, 131, -710),
    Vector3.new(2644, 129, -804),
    Vector3.new(2643, 128, -812),
    Vector3.new(2652, 129, -808),
    Vector3.new(2651, 128, -815),
    Vector3.new(2658, 129, -809),
    Vector3.new(2657, 128, -816),
    Vector3.new(2665, 129, -810),
    Vector3.new(2665, 128, -817),
    Vector3.new(2672, 129, -811),
    Vector3.new(2672, 128, -818),
    Vector3.new(2679, 129, -812),
    Vector3.new(2678, 128, -819),
    Vector3.new(2685, 129, -813),
    Vector3.new(2685, 128, -819),
    Vector3.new(2692, 129, -811),
    Vector3.new(2699, 129, -811),
    Vector3.new(2707, 129, -813)
    
    
}

            local deployTarget = CFrame.new(354.9398193359375, 131.8998565673828, 198.7338104248047, 
                                            -0.07539307326078415, 0, 0.9971538782119751, 
                                            0, 1, -0, 
                                            -0.9971538782119751, 0, -0.07539307326078415)

            -- ลูปผ่านแต่ละตำแหน่งและการปล่อย Crab Cage
            for index, position in ipairs(positions) do
                -- ตรวจสอบว่า _G.index เป็น false หรือไม่ ถ้าเป็น false จะหยุดลูป
                if not _G.index then
                    break
                end

                -- ย้ายตัวละครไปยังตำแหน่ง
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(position)
                
                -- ปล่อย Crab Cage
                local crabCage = game.Players.LocalPlayer.Character:FindFirstChild("Crab Cage")
                if crabCage and crabCage:FindFirstChild("Deploy") then
                    crabCage.Deploy:FireServer(deployTarget)

                end
                
                -- รอเวลาเล็กน้อยก่อนที่จะไปตำแหน่งถัดไป
                wait(0.3)
                
                -- ตรวจสอบว่าถึงตำแหน่งสุดท้ายแล้วหรือยัง
                if index == #positions then
                    _G.index = false
                   _G.indexV2 = true
                end
            end
        end
    end
end)
task.spawn(function()
    while true do
        task.wait(0.1)
        if _G.indexV2 then
 local targets = {
    {Vector3.new(2728, 133, -717), math.rad(170)},
    {Vector3.new(2720, 133, -719), math.rad(170)},
    {Vector3.new(2713, 133, -721), math.rad(170)},
    {Vector3.new(2705, 133, -722), math.rad(170)},
    {Vector3.new(2693, 132, -726), math.rad(150)},
    {Vector3.new(2687, 132, -729), math.rad(150)},
    {Vector3.new(2680, 132, -732), math.rad(150)},
    {Vector3.new(2665, 133, -741), math.rad(150)},
    {Vector3.new(2659, 133, -744), math.rad(150)},
    {Vector3.new(2653, 133, -748), math.rad(150)},
    {Vector3.new(2636, 130, -751), math.rad(170)},
    {Vector3.new(2633, 130, -755), math.rad(110)},
    {Vector3.new(2632, 130, -762), math.rad(110)},
    {Vector3.new(2632, 130, -767), math.rad(90)},
    {Vector3.new(2632, 130, -774), math.rad(90)},
    {Vector3.new(2632, 130, -782), math.rad(90)},
    {Vector3.new(2637, 133, -800), math.rad(100)},
    {Vector3.new(2636, 134, -807), math.rad(100)},
    {Vector3.new(2635, 135, -814), math.rad(100)},
    {Vector3.new(2634, 135, -821), math.rad(100)},
    {Vector3.new(2618, 131, -828), math.rad(190)},
    {Vector3.new(2611, 131, -828), math.rad(190)},
    {Vector3.new(2605, 131, -827), math.rad(190)},
    {Vector3.new(2598, 131, -830), math.rad(190)},
    {Vector3.new(2591, 131, -830), math.rad(190)},
    {Vector3.new(2584, 131, -829), math.rad(170)},
    {Vector3.new(2585, 131, -836), math.rad(80)},
    {Vector3.new(2586, 131, -843), math.rad(80)},
    {Vector3.new(2587, 131, -850), math.rad(80)},
    {Vector3.new(2589, 131, -858), math.rad(80)},
    {Vector3.new(2591, 131, -864), math.rad(80)},
    {Vector3.new(2592, 131, -871), math.rad(80)},
    {Vector3.new(2593, 131, -878), math.rad(80)},
    {Vector3.new(2595, 131, -886), math.rad(80)},
    {Vector3.new(2598, 131, -892), math.rad(80)},
    {Vector3.new(2600, 131, -899), math.rad(80)},
    {Vector3.new(2602, 130, -905), math.rad(0)},
    {Vector3.new(2608, 130, -913), math.rad(0)},
    {Vector3.new(2617, 131, -900), math.rad(10)},
    {Vector3.new(2623, 131, -901), math.rad(10)},
    {Vector3.new(2630, 131, -902), math.rad(10)}
}

            local deployTarget = CFrame.new(357.0093, 132, 201.9552, -0.084, 0, 0.996, 0, 1, 0, -0.996, 0, -0.084)

            for indexV2, target in ipairs(targets) do
                if not _G.indexV2 then break end

                -- สร้าง CFrame ใหม่จากตำแหน่งและการหมุน
                local targetCFrame = CFrame.new(target[1]) * CFrame.Angles(0, target[2], 0)

                -- ย้ายตัวละครไปยังตำแหน่งและหมุน
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = targetCFrame

                -- ปล่อย Crab Cage
                local crabCage = game.Players.LocalPlayer.Character:FindFirstChild("Crab Cage")
                if crabCage and crabCage:FindFirstChild("Deploy") then
                    crabCage.Deploy:FireServer(deployTarget)
                end

                task.wait(0.3)

                if indexV2 == #targets then
                    _G.indexV2 = false
                    _G.worldPivot = true
                end
            end
        end
    end
end)


_G.worldPivot = false
local isProcessing = false  -- ตัวแปรที่ใช้ในการตรวจสอบว่าโค้ดกำลังทำงานอยู่หรือไม่

local function startWorldPivot()
    -- ตรวจสอบว่าโค้ดกำลังทำงานอยู่หรือไม่
    if isProcessing then
        return  -- ถ้ามีการทำงานอยู่แล้วจะไม่เริ่มใหม่
    end

    isProcessing = true  -- ตั้งสถานะว่าเริ่มทำงานแล้ว

    while _G.worldPivot do
        task.wait(0.1)  -- Adding a small delay for efficiency

        local foundCrabCage = false

        -- Loop through crabcages
        for i = 1, 1000 do
            -- ตรวจสอบว่า _G.worldPivot ถูกตั้งเป็น false หรือไม่
            if not _G.worldPivot then
                isProcessing = false  -- การทำงานเสร็จสิ้นแล้ว
                return  -- ออกจากฟังก์ชันและหยุดการทำงานทันที
            end

            local crabcage = workspace.active.crabcages:GetChildren()[i]

            if crabcage and crabcage:IsA("Model") then
                -- If the model does not have PrimaryPart
                local part = crabcage:FindFirstChild("PrimaryPart") or crabcage:FindFirstChildOfClass("Part")
                if part then
                    -- Wait 1 second before moving to the next position
                    wait(0.1)

                    -- Teleport to the position of part
                    local worldPivotPosition = part.Position
                    game.Players.LocalPlayer.Character:SetPrimaryPartCFrame(CFrame.new(worldPivotPosition))
                    foundCrabCage = true
                end
            end
        end

        -- If no crabcages are found, print "Win"
        if not foundCrabCage then
            _G.index = true
            _G.worldPivot = false
        end
    end

    isProcessing = false  -- การทำงานเสร็จสิ้นแล้ว
end

-- ฟังก์ชันที่ใช้ในการเริ่มทำงาน
local function checkWorldPivot()
    if _G.worldPivot and not isProcessing then
        task.spawn(startWorldPivot)  -- เริ่มต้นการทำงานใหม่ถ้าไม่มีการทำงานอยู่
    end
end

-- เริ่มทำงานทันทีเมื่อ _G.worldPivot ถูกตั้งเป็น true
checkWorldPivot()

-- ใช้ RunService เพื่อให้ตรวจสอบตลอดเวลา
game:GetService("RunService").Heartbeat:Connect(function()
    checkWorldPivot()
end)








-- This script will run as long as _G.Tool is true, and it will start working when _G.Tool is set to true
task.spawn(function()
    while true do
        -- If _G.Tool is true, start the loop to equip the "Crab Cage"
        if _G.Tool1 then
            local player = game.Players.LocalPlayer
            local backpack = player.Backpack

            -- Check if the "Crab Cage" exists in the backpack
            local crabCage = backpack:FindFirstChild("Crab Cage")

            if crabCage then
                -- Equip the "Crab Cage" item
                player.Character:WaitForChild("Humanoid"):EquipTool(crabCage)
            else
                print("Crab Cage not found in backpack.")
            end
        end

        -- Short delay before the next loop iteration to prevent freezing
        task.wait(0)
    end
end)

if not _G.Autoprompt then
    _G.Autoprompt = false  -- กำหนดค่าเริ่มต้นให้เป็น false
end

task.spawn(function()
    while true do  -- ลูปแบบต่อเนื่อง
        task.wait(0)  -- หยุดรอสั้นๆ เพื่อหลีกเลี่ยงการแฮงค์

        if _G.Autoprompt then
            -- จำลองการกดและปล่อยปุ่ม "E"
            game:GetService('VirtualInputManager'):SendKeyEvent(true, Enum.KeyCode.E, false, game)
            task.wait(0)
            game:GetService('VirtualInputManager'):SendKeyEvent(false, Enum.KeyCode.E, false, game)

            -- ดึง Crabcages ทั้งหมดใน collection
            local crabcages = workspace.active.crabcages:GetChildren()

            -- ลูปไปที่ Crabcages (ไม่เกิน 1000 อัน)
            for i = 1, math.min(1000, #crabcages) do
                local crabcage = crabcages[i]  -- เข้าถึง Crabcage ที่ตำแหน่ง i
                if crabcage then
                    local prompt = crabcage:FindFirstChild("Prompt")  -- หา Prompt ใน Crabcage
                    if prompt then
                        prompt.HoldDuration = 0  -- ตั้ง HoldDuration เป็น 0
                        prompt.MaxActivationDistance = 100  -- ตั้ง MaxActivationDistance เป็น 100
                    end
                end
            end
        end
    end
end)




---//---//----//---//---//----//---//---//----//---//---//----//---//---//----//
local Fluent = loadstring(game:HttpGet("https://github.com/dawid-scripts/Fluent/releases/latest/download/main.lua"))()
local SaveManager = loadstring(game:HttpGet("https://raw.githubusercontent.com/dawid-scripts/Fluent/master/Addons/SaveManager.lua"))()
local InterfaceManager = loadstring(game:HttpGet("https://raw.githubusercontent.com/dawid-scripts/Fluent/master/Addons/InterfaceManager.lua"))()

local Window = Fluent:CreateWindow({
    Title = "XXX hub [FREE]",
    SubTitle = "by 999",
    TabWidth = 160,
    Size = UDim2.fromOffset(555, 355),
    Acrylic = true, -- The blur may be detectable, setting this to false disables blur entirely
    Theme = "Values",
    MinimizeKey = Enum.KeyCode.LeftControl -- Used when theres no MinimizeKeybind
})

--Fluent provides Lucide Icons https://lucide.dev/icons/ for the tabs, icons are optional
local Tabs = {
    AutoFishing = Window:AddTab({ Title = "Auto Fishing", Icon = "home" }),
    Farm = Window:AddTab({ Title = "Farm", Icon = "gem" }),
    Event = Window:AddTab({ Title = "Event", Icon = "fan" }),
    Enchant = Window:AddTab({ Title = "Enchant", Icon = "mountain" }),
    file = Window:AddTab({ Title = "Teleport to File", Icon = "file" }),
    Players = Window:AddTab({ Title = "Players", Icon = "user" }),
    Miscellaneous = Window:AddTab({ Title = "Miscellaneous", Icon = "align-justify" }),
    Shop = Window:AddTab({ Title = "Shop", Icon = "shopping-cart" }),
    Fake = Window:AddTab({ Title = "Fake", Icon = "chevrons-up" }),
    Trading = Window:AddTab({ Title = "Trading", Icon = "refresh-cw" }),
    Server = Window:AddTab({ Title = "Server", Icon = "hard-drive" }),
    Settings = Window:AddTab({ Title = "Settings", Icon = "settings" })
}

  local section = Tabs.AutoFishing:AddSection("Fishing Bot")
  local section = Tabs.Farm:AddSection("Level Farm")
  local section = Tabs.Players:AddSection("Movement")
  local section = Tabs.Fake:AddSection("FakeUp")  
  local section = Tabs.Miscellaneous:AddSection("Misc")
  local section = Tabs.Server:AddSection("Server")
  local section = Tabs.Trading:AddSection("Trading Options")

local Options = Fluent.Options

do
local Toggle = Tabs.AutoFishing:AddToggle("MyToggle", {
    Title = "Auto Fishing", 
    Default = false, 
    Description = "Automatically fish for you."  -- Adding description to the toggle
})

Toggle:OnChanged(function()
    _G.Tool1234 = Toggle.Value

    if _G.Tool1234  then
        task.spawn(function()
            while _G.Tool1234  do
                task.wait(0)  -- Added a small delay to reduce unnecessary checks


          local player = game:GetService("Players").LocalPlayer
local backpack = player.Backpack

-- Check for tools in the player's backpack
for _, item in pairs(backpack:GetChildren()) do
    if item:IsA("Tool") and string.find(item.Name, "Rod") then
        -- Ensure the item is not "Crab Cage" before equipping
        if item.Name ~= "Crab Cage" then
            local humanoid = player.Character:WaitForChild("Humanoid")
            humanoid:EquipTool(item)  -- Equip the rod item
            break  -- Stop searching after finding the first match
        end
    end
end

-- Check for tools in the player's character (not workspace.D3B3XxX)
local rodItem = nil
for _, item in pairs(player.Character:GetChildren()) do
    if item:IsA("Tool") and string.find(item.Name, "Rod") then
        -- Ensure the item is not "Crab Cage" before equipping
        if item.Name ~= "Crab Cage" then
            rodItem = item  -- Found the rod in the character, not the "Crab Cage"
            break  -- Stop searching after finding the first match
        end
    end
end

-- If a "Rod" item is found in the player's character, trigger the cast event
if rodItem then
    local events = rodItem:FindFirstChild("events")
    if events and events:FindFirstChild("cast") then
        -- Fire the cast event with arguments
        local args = {
            [1] = 99999999999999,
            [2] = 1
        }
        events.cast:FireServer(unpack(args))
    end
end

task.wait(0)  -- Add delay to prevent overloading the server

            end
        end)
    end
end)

            end
local Toggle = Tabs.AutoFishing:AddToggle("MyToggle", {
    Title = "Auto Use Bait", 
    Default = false, 
    Description = "Automatically use vait when fishing."  -- Adding description to the toggle
})
    Toggle:OnChanged(function()
 
    end)
    

      local MultiDropdown = Tabs.AutoFishing:AddDropdown("MultiDropdown", {
        Title = "Select Bait",
        Description = "",
        Values = {"Magnet", "Worm", "Peppermint Worm", "Coal", "Squid", "Shrimp", "Insect", "Give", "Night Shrimp", "Deep Coral", "Super Flakes", "Swaweed", "Instant", "Shark Head", "Fish Head", "Weird Algae", "Garbage",  "Holly Berry", "Rapid Catcher", "Minnow", "Coral", "Flakes", "Aurora Bait", "Bagel", "Truffle Worm"},
        Multi = true,
        Default = {"seven", "twelve"},
    })

    MultiDropdown:SetValue({
        three = true,
        five = true,
        seven = false
    })

    MultiDropdown:OnChanged(function(Value)
        local Values = {}
        for Value, State in next, Value do
            table.insert(Values, Value)
        end
    end)

local Toggle = Tabs.AutoFishing:AddToggle("MyToggle", {
    Title = "Auto FastShake", 
    Default = false, 
    Description = "Automatically FastShake the rod."
})

Toggle:OnChanged(function(se)
    _G.FastShake = se
if not _G.FastShake then
    _G.FastShake = false
end

-- ฟังก์ชันหลักที่ทำงานตลอดเวลา
task.spawn(function()
    while true do
        task.wait(0)  -- หยุดรอสั้นๆ เพื่อหลีกเลี่ยงการแฮงค์

        -- ถ้าค่า _G.FastShake เป็น true ให้ทำงาน
        if _G.FastShake then
            -- ลูปเพื่อจำลองการคลิกปุ่ม 10,000 ครั้ง
            for i = 1, 3 do
                -- เลือกผู้เล่นและ GUI ที่เกี่ยวข้อง
                local player = game.Players.LocalPlayer
                local GUI = player:WaitForChild("PlayerGui")
                local shakeui = GUI:WaitForChild("shakeui")
                local VirtualInputManager = game:GetService("VirtualInputManager")
                local button = shakeui.safezone:FindFirstChild("button")

                -- ถ้าปุ่มอยู่และเป็น ImageButton, จำลองการคลิก
                if button and button:IsA("ImageButton") then
                    -- เลือกปุ่มและจำลองการคลิก
                    game:GetService("GuiService").SelectedCoreObject = button
                    VirtualInputManager:SendKeyEvent(true, Enum.KeyCode.Return, false, game)
                    VirtualInputManager:SendKeyEvent(false, Enum.KeyCode.Return, false, game)
                end
            end
        end
    end
end)
end)


local Toggle = Tabs.AutoFishing:AddToggle("MyToggle", {
    Title = "Auto Shake", 
    Default = true, 
    Description = "Automatically Shake the rod."
})

Toggle:OnChanged(function(value)
    _G.Autoshake = value


if not _G.Autoshake then
    _G.Autoshake = false
end

-- ฟังก์ชันหลักที่ทำงานตลอดเวลา
task.spawn(function()
    while true do
        task.wait(0)  -- หยุดรอสั้นๆ เพื่อหลีกเลี่ยงการแฮงค์

        -- ถ้าค่า _G.FastShake เป็น true ให้ทำงาน
        if _G.Autoshake then
            -- ลูปเพื่อจำลองการคลิกปุ่ม 10,000 ครั้ง
                    local player = game.Players.LocalPlayer
                    local GUI = player:WaitForChild("PlayerGui")
                    local shakeui = GUI:WaitForChild("shakeui")
                    local VirtualInputManager = game:GetService("VirtualInputManager")

                    -- Locate the button and interact with it
                    local button = shakeui.safezone:FindFirstChild("button")
                    if button and button:IsA("ImageButton") and button.Visible then
                        game:GetService("GuiService").SelectedCoreObject = button
                        VirtualInputManager:SendKeyEvent(true, Enum.KeyCode.Return, false, game)
                        VirtualInputManager:SendKeyEvent(false, Enum.KeyCode.Return, false, game)
                    end
                end
            end
        end)
    end)
    






local Toggle = Tabs.AutoFishing:AddToggle("MyToggle", {
    Title = "Auto Reel", 
    Default = false, 
    Description = "Automatically finish the fishinf process."  -- Adding description to the toggle
})
    Toggle:OnChanged(function()
_G.AutoReel1 = Toggle.Value
_G.AutoReel2 = Toggle.Value

   if _G.AutoReel1 then
            task.spawn(function()
                while _G.AutoReel1 do
                    task.wait(0)
                    local reelfinished = game:GetService("ReplicatedStorage"):WaitForChild("events"):WaitForChild("reelfinished")
                    local LocalPlayer = game.Players.LocalPlayer

                    for _, v in pairs(LocalPlayer.PlayerGui:GetChildren()) do
                        if v:IsA("ScreenGui") and v.Name == "reel" then
                            if v:FindFirstChild("bar") then
                                reelfinished:FireServer(100, true)
                            end
                        end
                    end
                end
            end)
        end

        -- Auto Reel 2 logic
        if _G.AutoReel2 then
            task.spawn(function()
                while _G.AutoReel2 do
                    task.wait(0)
                    local reelfinished = game:GetService("ReplicatedStorage").Link.events.reelfinished
                    local LocalPlayer = game.Players.LocalPlayer

                    for _, v in pairs(LocalPlayer.PlayerGui:GetChildren()) do
                        if v:IsA("ScreenGui") and v.Name == "reel" then
                            if v:FindFirstChild("bar") then
                                reelfinished:FireServer(100, true)
                            end
                        end
                    end
                end
            end)
        end
    end)
    
local Toggle = Tabs.AutoFishing:AddToggle("MyToggle", {
    Title = "AutoReelSafe", 
    Default = true, 
    Description = "Automatically finish the fishinf process [Safe]."  -- Adding description to the toggle
})

Toggle:OnChanged(function()
    _G.AutoReel3 = Toggle.Value
    
    if _G.AutoReel3 then
        task.spawn(function()
            while _G.AutoReel3 do
                task.wait(0)  -- Adding a slight delay to prevent overloading the system
                
                local player = game:GetService("Players").LocalPlayer
                local playerGui = player:FindFirstChild("PlayerGui")
                
                -- Check if playerGui, reel, bar, and playerbar exist
                if playerGui and playerGui:FindFirstChild("reel") and 
                   playerGui.reel:FindFirstChild("bar") and 
                   playerGui.reel.bar:FindFirstChild("playerbar") then
                   
                    local playerBar = playerGui.reel.bar.playerbar
                    local fish = playerGui.reel.bar:FindFirstChild("fish")
                    
                    -- Check if fish exists before changing the position
                    if fish then
                        playerBar.Position = fish.Position
                    end
                end
            end
        end)
    end
end)

  local section = Tabs.AutoFishing:AddSection("Fishing Positions")
-- สร้าง Paragraph
local paragraph = Tabs.AutoFishing:AddParagraph({
    Title = "X Y Z: Initializing...",
    Content = ""
})

-- ฟังก์ชันอัพเดตตำแหน่ง xyz
local function updateLevel()
    local player = game.Players.LocalPlayer -- รับข้อมูลผู้เล่นที่รันสคริปต์
    local character = player.Character or player.CharacterAdded:Wait() -- รับตัวละครของผู้เล่น
    
    -- ใช้ pcall เพื่อป้องกันข้อผิดพลาด
    pcall(function()
        while true do
            -- ตรวจสอบว่าตัวละครมี HumanoidRootPart หรือไม่
            if character:FindFirstChild("HumanoidRootPart") then
                local position = character.HumanoidRootPart.Position -- ตำแหน่งของ HumanoidRootPart
                local x, y, z = math.floor(position.X), math.floor(position.Y), math.floor(position.Z) -- ปัดตำแหน่งเป็นตัวเลขเต็ม
                paragraph:SetTitle("X Y Z : " .. tostring(x) .. ", " .. tostring(y) .. ", " .. tostring(z)) -- อัพเดต Title
            else
                paragraph:SetTitle("xyz: Waiting for position...") -- กรณีที่ยังไม่มีตำแหน่ง
            end
            task.wait(0) -- อัพเดตทุก 0.5 วินาที
        end
    end)
end

-- เรียกใช้งานฟังก์ชันอัพเดต
task.spawn(updateLevel) -- แก้ไขให้ task.spawn เรียกใช้ฟังก์ชันโดยไม่ใส่วงเล็บ


local targetPosition = nil -- ตัวแปรสำหรับเก็บตำแหน่ง
local targetOrientation = CFrame.new() -- ตัวแปรสำหรับเก็บทิศทาง (ค่าเริ่มต้นเป็น CFrame ว่าง)
local shouldStop = false -- ใช้ควบคุมการวาร์ป

-- Toggle สำหรับการวาร์ป
local Toggle = Tabs.AutoFishing:AddToggle("MyToggle", {
    Title = "Teleport To Position",
    Default = false,
    Description = "Automatically teleport to your saved position." -- เพิ่มคำอธิบาย
})

Toggle:OnChanged(function(state)
    local player = game.Players.LocalPlayer
    local character = player.Character or player.CharacterAdded:Wait()
    local humanoidRootPart = character:WaitForChild("HumanoidRootPart")

    if not humanoidRootPart then
        warn("HumanoidRootPart not found!")
        return
    end

    if state then
        -- ถ้า Toggle เปิด
        if targetPosition then
            shouldStop = false
            while not shouldStop do
                humanoidRootPart.CFrame = CFrame.new(targetPosition) * targetOrientation
                task.wait(0)
            end
        end
    else
        -- ถ้า Toggle ปิด
        shouldStop = true
    end
end)

-- ปุ่มสำหรับตั้งค่าตำแหน่งและทิศทาง
Tabs.AutoFishing:AddButton({
    Title = "Set Fishing Position and Direction",
    Description = "Set your new fishing position and direction",
    Callback = function()
        local player = game.Players.LocalPlayer
        local humanoidRootPart = player.Character and player.Character:FindFirstChild("HumanoidRootPart")

        if not humanoidRootPart then
            return
        end

        -- เก็บตำแหน่งปัจจุบัน
        local position = humanoidRootPart.Position
        local x, y, z = position.X, position.Y, position.Z

        -- ตรวจสอบว่าค่าทั้งหมดไม่เป็น nil
        if not x or not y or not z then
            return
        end

        -- เก็บทิศทางปัจจุบัน (Rotation)
        local rx, ry, rz = humanoidRootPart.CFrame:ToEulerAnglesYXZ()

        -- บันทึกค่าที่เก็บไว้ในตัวแปร
        targetPosition = Vector3.new(x, y, z)
        targetOrientation = CFrame.Angles(rx, ry, rz)

        -- คัดลอกข้อมูลตำแหน่งไปยังคลิปบอร์ด
        local positionString = string.format("Position: %.2f, %.2f, %.2f", x, y, z)
        setclipboard(positionString)
    end
})


-- สร้าง Paragraph


-- สร้าง Toggle
local Toggle = Tabs.Farm:AddToggle("MyToggle", {
    Title = "AutoLevelFarm", 
    Default = false, 
    Description = "Auto Level Farm."
})
local ScreenGui -- ตัวแปรที่จะเก็บ UI

Toggle:OnChanged(function(state)
    -- เปิดหรือปิดการทำงานตามค่าของ state
    _G.index = state
    _G.Tool1 = state
    _G.Autoprompt = state
    _G.worldPivot = state
    _G.indexV2 = state
    _G.indexV2 = false

    if state then
        -- เริ่มการทำงานของแต่ละฟังก์ชัน
        task.spawn(function()
            while _G.index do
                task.wait(0.1)
                -- โค้ดสำหรับการจัดการ `_G.index`

            end
        end)

        task.spawn(function()
            while _G.indexV2 do 
                task.wait(0.1)
                -- โค้ดสำหรับการจัดการ `_G.indexV2`

            end
        end)

        task.spawn(function()
            while _G.Tool1 do 
                task.wait(0.1)
                -- โค้ดสำหรับการจัดการ `_G.ToolCrab`

            end
        end)

        task.spawn(function()
            while _G.Autoprompt do
                task.wait(0.1)
                -- โค้ดสำหรับการจัดการ `_G.Autoprompt`

            end
        end)

        task.spawn(function()
            while _G.worldPivot do
                task.wait(0.1)
                -- โค้ดสำหรับการจัดการ `_G.worldPivot`

            end
        end)

        -- สร้าง UI เมื่อ Toggle เปิด
        ScreenGui = Instance.new("ScreenGui")
        ScreenGui.Parent = game.Players.LocalPlayer.PlayerGui

        -- สร้าง Frame
        local Frame = Instance.new("Frame")
        Frame.Size = UDim2.new(0, 400, 0, 200)  -- ขนาดของกรอบ
        Frame.Position = UDim2.new(0.5, -200, 0.5, -100)  -- ตำแหน่งของกรอบ
        Frame.BackgroundColor3 = Color3.fromRGB(0, 0, 0)  -- สีพื้นหลัง
        Frame.BackgroundTransparency = 1  -- ความโปร่งใส
        Frame.Parent = ScreenGui

        -- เพิ่ม UICorner เพื่อทำมุมโค้งให้กับ Frame
        local UICorner = Instance.new("UICorner")
        UICorner.CornerRadius = UDim.new(0, 15)  -- มุมโค้ง
        UICorner.Parent = Frame

        -- สร้าง TextLabel ที่แสดงตัวอักษร  
        local TextLabel = Instance.new("TextLabel")
        TextLabel.Size = UDim2.new(0, 200, 0, 50)  -- ขนาดของข้อความ
        TextLabel.Position = UDim2.new(0.5, -100, 0, 0)  -- ตำแหน่งของข้อความ (อยู่ด้านบนสุด)
        TextLabel.BackgroundTransparency = 1  -- ทำให้พื้นหลังโปร่งใส
        TextLabel.Text = "🟢 star : Level Farm"  -- ข้อความที่จะแสดง (ตัวอักษร)
        TextLabel.TextColor3 = Color3.fromRGB(255, 0, 0)  -- สีข้อความ
        TextLabel.TextSize = 20  -- ขนาดข้อความที่เล็กลง
        TextLabel.Parent = Frame

    else  -- ถ้า Toggle ปิด
        -- ลบ UI ถ้า Toggle ปิด
        if ScreenGui then
            ScreenGui:Destroy()  -- ลบ ScreenGui ถ้ามี
            ScreenGui = nil  -- รีเซ็ตตัวแปร ScreenGui
        end

    end

    -- เริ่มทำงานการฟาร์ม เมื่อ Toggle เปิด
    if _G.Farm then
        task.spawn(function()
            while _G.Farm do
                task.wait(1)  -- เพิ่มเวลาหน่วงเพื่อให้ไม่กระทบกับประสิทธิภาพ
                -- ฟังก์ชันที่คุณต้องการให้ทำงานเมื่อ Toggle เปิด
                print("...กำลังฟาร์ม")
            end
        end)
    end
end)
local Toggle = Tabs.Farm:AddToggle("MyToggle", {
    Title = "BuyCrab", 
    Default = false, 
    Description = "Auto Buy Crab."
})

-- Add a toggle to the Farm tab
Toggle:OnChanged(function(state)
    _G.BuyCrab = state
    if state then
        -- Start the auto-buy process
        task.spawn(function()
            while _G.BuyCrab do
                task.wait(0) -- Prevent overwhelming the system
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(2526, 136, -893) 

                -- Simulate pressing the 'E' key
                game:service('VirtualInputManager'):SendKeyEvent(true, "E", false, game)
                game:service('VirtualInputManager'):SendKeyEvent(false, "E", false, game)
                
                -- Check for the 'prompt' GUI element
                local playerGui = game:GetService("Players").LocalPlayer.PlayerGui
                if playerGui:FindFirstChild("over") and playerGui.over:FindFirstChild("prompt") then
                    local prompt = playerGui.over.prompt
                    if prompt:FindFirstChild("confirm") then
                        -- Trigger the confirmation button
                        for _, connection in pairs(getconnections(prompt.confirm.MouseButton1Click)) do
                            if connection.Function then
                                connection.Function()
                            end
                        end
                    end
                end
            end
        end)
    end
end)


local rodsFarmSection = Tabs.Farm:AddSection("ฟาร์มคันเบ็ด")  -- แสดงเป็นภาษาไทย

local AutoTridentRod = rodsFarmSection:AddToggle("AutoTridentRod", {
    Title = "ฟาร์มไตรเดนท์อัตโนมัติ",  -- แสดงเป็นภาษาไทย
    Default = _G.Toggle,
    Description = "เปิดใช้งานการฟาร์มคันเบ็ดไตรเดนท์โดยอัตโนมัติ"
})

local AutoAuroraRod = rodsFarmSection:AddToggle("AutoAuroraRod", {
    Title = "ฟาร์มออโรร่าอัตโนมัติ",  -- แสดงเป็นภาษาไทย
    Default = false,
    Description = "เปิดใช้งานการฟาร์มคันเบ็ดออโรร่าโดยอัตโนมัติ"
})

local AutoKingsRod = rodsFarmSection:AddToggle("AutoKingsRod", {
    Title = "ฟาร์มคิงส์อัตโนมัติ",  -- แสดงเป็นภาษาไทย
    Default = false,
    Description = "เปิดใช้งานการฟาร์มคันเบ็ดคิงส์โดยอัตโนมัติ"
})

local AutoDestinyRod = rodsFarmSection:AddToggle("AutoDestinyRod", {
    Title = "ฟาร์มเดสทินีอัตโนมัติ",  -- แสดงเป็นภาษาไทย
    Default = false,
    Description = "เปิดใช้งานการฟาร์มคันเบ็ดเดสทินีโดยอัตโนมัติ"
})

local AutoMythicalRod = rodsFarmSection:AddToggle("AutoMythicalRod", {
    Title = "ฟาร์มมิธิคอลอัตโนมัติ",  -- แสดงเป็นภาษาไทย
    Default = false,
    Description = "เปิดใช้งานการฟาร์มคันเบ็ดมิธิคอลโดยอัตโนมัติ"
})


function buy1()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-932, 226, -991)
wait(5)
local merlinPower = workspace.world.npcs.Merlin.Merlin.power

if merlinPower and merlinPower.InvokeServer then
    for i = 1, 5 do
        local success, result = pcall(function()
            return merlinPower:InvokeServer()
        end)

        if success then
            if result then
            else
            end
        end
    end
end
end


function Enchant()
local player = game:GetService("Players").LocalPlayer
local enchantRelic = player.Backpack:FindFirstChild("Enchant Relic")

if enchantRelic and enchantRelic:IsA("Tool") then
    player.Character.Humanoid:EquipTool(enchantRelic)
   end
end


 

function E2()
				game:service('VirtualInputManager'):SendKeyEvent(true, "E", false, game)
                task.wait(0)
				game:service('VirtualInputManager'):SendKeyEvent(false, "E", false, game)
end
function prompt()
for _, prompt in ipairs(workspace:GetDescendants()) do
    if prompt:IsA("ProximityPrompt") then
        prompt.HoldDuration = 0  -- ตั้ง HoldDuration เป็น 0
        prompt.MaxActivationDistance = 100  -- ตั้ง MaxActivationDistance เป็น 100
    end
end
end


spawn(function()
    while task.wait(0) do
        pcall(function()
        if _G.E then

            E2()
           end
        end)
    end
end)

spawn(function()
    while task.wait(0) do
        pcall(function()
        if _G.prompt then

            prompt()
           end
        end)
    end
end)


AutoTridentRod:OnChanged(function(value)
    if value then
        local player = game.Players.LocalPlayer
        local character = player.Character or player.CharacterAdded:Wait()
        
        -- ยกเลิกการถืออาวุธทั้งหมด
        for _, tool in ipairs(character:GetChildren()) do
            if tool:IsA("Tool") then
                tool.Parent = player.Backpack -- นำไอเท็มกลับไปที่กระเป๋า
            end
        end

        local backpack = player.Backpack
        if not backpack:FindFirstChild("Trident Rod") then
            game:GetService("ReplicatedStorage"):WaitForChild("packages"):WaitForChild("Net"):WaitForChild("RE/Rod/Equip"):FireServer("Trident Rod")
            wait(0.1)
        end
        
        if backpack:FindFirstChild("Trident Rod") then
            AutoTridentRod:SetValue(false)
        else
            buy1()
            _G.E = true
            wait(6)
            E2()
            wait(1)
            Enchant()
            E2()

            -- ลำดับการเคลื่อนที่เพื่อทำ Enchant ซ้ำๆ
            local positions = {
                Vector3.new(-1464.96, -221.73, -2328.54),
                Vector3.new(-1471.13, -221.73, -2331.64),
                Vector3.new(-1479.41, -221.73, -2333.04),
                Vector3.new(-1487.59, -221.74, -2332.75),
                Vector3.new(-1493.40, -221.73, -2329.21),
            }

            for _, pos in ipairs(positions) do
                _G.prompt = true
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(pos)
                wait(3)
                Enchant()
                E2()
            end

            wait(5)
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1484.65, -223.49, -2195.60)
            local VirtualInputManager = game:GetService('VirtualInputManager')

            -- กดปุ่ม E เพื่อดำเนินการ
            VirtualInputManager:SendKeyEvent(true, "E", false, game)
            task.wait(0.005)
            VirtualInputManager:SendKeyEvent(false, "E", false, game)
            _G.prompt = false

            -- ตรวจสอบ UI และกดปุ่มยืนยันถ้ามี
            task.wait(0.1)
            local overGui = player.PlayerGui:FindFirstChild("over")
            if overGui and overGui:FindFirstChild("prompt") and overGui.prompt:FindFirstChild("confirm") then
                for _, connection in pairs(getconnections(overGui.prompt.confirm.MouseButton1Click)) do
                    if connection.Function then
                        connection.Function()
                        wait(3)
                    end
                end
            end
        end
    end
end)



-- Add a toggle to the Farm tab
local Toggle = Tabs.Players:AddToggle("MyToggle", {
    Title = "Walk Speed", 
    Default = true, 
    Default = false, 
    Description = "You can run at high speed."
})

Toggle:OnChanged(function(State)
    if State then
        _G.WalkSpeed = true
    else
        local player = game.Players.LocalPlayer
        local humanoid = player.Character and player.Character:FindFirstChild("Humanoid")
        
        -- รีเซ็ต WalkSpeed เป็น 16 เมื่อปิด
        if humanoid then
            humanoid.WalkSpeed = 16
        end
        _G.WalkSpeed = false
    end
end)



-- Create Slider for adjusting WalkSpeed
local Slider = Tabs.Players:AddSlider("Slider", {
    Title = "WalkSpeed Slider",
    Description = "Adjust running speed.",
    Default = 16,  -- Default WalkSpeed (Roblox default is 16)
    Min = 1,
    Max = 200,  -- Maximum WalkSpeed (adjustable)
    Rounding = 1,
    Callback = function(Value)
        -- ตรวจสอบว่า _G.WalkSpeed เป็น true ก่อนจะอัปเดต WalkSpeed
        if _G.WalkSpeed then
            local player = game.Players.LocalPlayer
            local humanoid = player.Character and player.Character:FindFirstChild("Humanoid")
            
            -- อัปเดต WalkSpeed หาก humanoid มีอยู่
            if humanoid then
                humanoid.WalkSpeed = Value
            end
        end
    end
})

Slider:OnChanged(function(Value)
    -- Optionally log or do something else when the slider value changes
    -- print("Slider Value: " .. Value)
end)

local Toggle = Tabs.Players:AddToggle("MyToggle", {
    Title = "Jump Power", 
    Default = true, 
    Default = false, 
    Description = "You can jump power."
})

Toggle:OnChanged(function(State)
    if State then
        _G.JumpPower = true
    else
        local player = game.Players.LocalPlayer
        local humanoid = player.Character and player.Character:FindFirstChild("Humanoid")
        
        -- รีเซ็ต WalkSpeed เป็น 16 เมื่อปิด
        if humanoid then
            humanoid.JumpPower = 16
        end
        _G.JumpPower = false
    end
end)



local Slider = Tabs.Players:AddSlider("Slider", {
    Title = "Jump Power",
    Description = "Adjust jump power.",
    Default = 50,  -- ค่าเริ่มต้นของ JumpPower
    Min = 1,
    Max = 500,  -- ความสูงการกระโดดสูงสุด
    Rounding = 1,
    Callback = function(Value)
        -- ตรวจสอบว่า _G.JumpPower เป็น true ก่อนจะอัปเดต JumpPower
        if _G.JumpPower then
            local player = game.Players.LocalPlayer
            local humanoid = player.Character and player.Character:FindFirstChild("Humanoid")
            
            -- อัปเดต JumpPower หาก humanoid มีอยู่
            if humanoid then
                humanoid.JumpPower = Value
            end
        end
    end
})

local Toggle = Tabs.Players:AddToggle("MyToggle", {
    Title = "infinite oxygen", 
    Default = true, 
    Default = false, 
    Description = "You can infinite oxygen."
})

Toggle:OnChanged(function(state)
    local character = game.Players.LocalPlayer.Character
    if character and character:FindFirstChild("client") then
        local oxygen = character.client:FindFirstChild("oxygen")
        if oxygen then
            -- เมื่อ Toggle เปิดให้ปิด oxygen, เมื่อ Toggle ปิดให้เปิด oxygen
            oxygen.Enabled = not state
        end
    end
end)


local Toggle = Tabs.Players:AddToggle("MyToggle", {
    Title = "Infinite Oxygen (Peaks)",
    Default = false,
    Description = "You can infinite oxygen(peaks)."
})

Toggle:OnChanged(function(state)
    local player = game.Players.LocalPlayer.Character
    if player and player:FindFirstChild("client") then
        local oxygenPeaks = player.client:FindFirstChild("oxygen(peaks)") -- ค้นหา "oxygen(peaks)"
        if oxygenPeaks then
            -- เมื่อ Toggle เปิดให้ปิด oxygen, เมื่อ Toggle ปิดให้เปิด oxygen
            oxygenPeaks.Enabled = not state
        end
    end
end)

local Toggle = Tabs.Players:AddToggle("MyToggle", {
    Title = "Infinite temperature",
    Default = false,
    Description = "You can infinite temperature."
})

Toggle:OnChanged(function(state)
    local player =game.Players.LocalPlayer.Character
    if player and player:FindFirstChild("client") then
        local temperature = player.client:FindFirstChild("temperature") -- ค้นหา "temperature"
        if temperature then
            -- เมื่อ Toggle เปิดให้ปิด temperature, เมื่อ Toggle ปิดให้เปิด temperature
            temperature.Enabled = not state
        end
    end
end)




local Toggle = Tabs.Miscellaneous:AddToggle("MyToggle", {
    Title = "Auto Sell", 
    Default = true, 
    Default = false, 
    Description = "You can auto sell hand."
})

    Toggle:OnChanged(function(ez)

    _G.Sell  = ez

if not _G.Sell then
    _G.Sell = false  -- กำหนดค่าเริ่มต้นให้เป็น false
end

task.spawn(function()
    while true do  -- ลูปแบบต่อเนื่อง
        task.wait(0)  -- หยุดรอสั้นๆ เพื่อหลีกเลี่ยงการแฮงค์

        if _G.Sell then

game:GetService("ReplicatedStorage"):WaitForChild("events"):WaitForChild("Sell"):InvokeServer()



end
end
end)


    end)
    local Toggle = Tabs.Miscellaneous:AddToggle("MyToggle", {
    Title = "Auto Sell all", 
    Default = true, 
    Default = false, 
    Description = "You can auto sell all."
})

    Toggle:OnChanged(function(ez1)

    _G.Sell1  = ez1

if not _G.Sell1 then
    _G.Sell1 = false  -- กำหนดค่าเริ่มต้นให้เป็น false
end

task.spawn(function()
    while true do  -- ลูปแบบต่อเนื่อง
        task.wait(0)  -- หยุดรอสั้นๆ เพื่อหลีกเลี่ยงการแฮงค์

        if _G.Sell1 then

game:GetService("ReplicatedStorage"):WaitForChild("events"):WaitForChild("SellAll"):InvokeServer()



end
end
end)


    end)





    local Toggle = Tabs.Trading:AddToggle("MyToggle", {
    Title = "Auto Accept Trade", 
    Default = false, 
    Description = "Press Accept ltem for the ltems traded by another player."
})

    Toggle:OnChanged(function(V)
_G.AutoTrade = V

if not _G.AutoTrade then
    _G.AutoTrade = false  -- กำหนดค่าเริ่มต้นให้เป็น false
end

task.spawn(function()
    while true do  -- ลูปแบบต่อเนื่อง
        task.wait(0)  -- หยุดรอสั้นๆ เพื่อหลีกเลี่ยงการแฮงค์

        if _G.AutoTrade then




local player = game:GetService("Players").LocalPlayer
local bodyAnnouncements = player.PlayerGui.hud.safezone:FindFirstChild("bodyannouncements")

if bodyAnnouncements and bodyAnnouncements:FindFirstChild("offer") then
    local confirmButton = bodyAnnouncements.offer.confirm
    for _, connection in pairs(getconnections(confirmButton.MouseButton1Click)) do
        connection.Function(confirmButton)
    end
end
end
end
end)
    end)


local Toggle = Tabs.Fake:AddToggle("MyToggle", {Title = "coins up", Default = false })

Toggle:OnChanged(function(e)
    -- Set the global variable based on toggle state
    _G.coinsFake = e

    -- Make sure _G.coinsFake defaults to false if it's not already set
    if not _G.coinsFake then
        _G.coinsFake = false  -- กำหนดค่าเริ่มต้นให้เป็น false
    end

    -- Create a new thread to continuously check the toggle state
    task.spawn(function()
        while true do  -- Loop indefinitely
            task.wait(0.1)  -- Small delay to avoid performance issues

            if _G.coinsFake then
                -- Get the player's coin value
                local player = game.Players.LocalPlayer
                local coins = game:GetService("ReplicatedStorage"):WaitForChild("playerstats"):WaitForChild(player.Name):WaitForChild("Stats"):WaitForChild("coins")

                -- Increment the coin value by 1
                coins.Value += _G.coinsIncrease
            end
        end
    end)
end)




local Slider = Tabs.Fake:AddSlider("Slider", {
    Title = "coins",
    Description = "",
    Default = 2,
    Min = 1,
    Max = 10000000000,
    Rounding = 1,
    Callback = function(Value)
        print("Slider was changed:", Value)
        _G.coinsIncrease = Value  -- อัพเดทค่าการเพิ่ม coins จาก Slider
    end
})


Tabs.Fake:AddButton({
    Title = "coins up",
    Description = "not loop",
    Callback = function()
   -- Get the player's coin value
                local player = game.Players.LocalPlayer
                local coins = game:GetService("ReplicatedStorage"):WaitForChild("playerstats"):WaitForChild(player.Name):WaitForChild("Stats"):WaitForChild("coins")

                -- Increment the coin value by 1
                coins.Value += _G.coinsIncrease
    end
})



local Toggle = Tabs.Fake:AddToggle("MyToggle", {Title = "level up", Default = false })

Toggle:OnChanged(function(e)
    -- Set the global variable based on toggle state
    _G.levelFake = e

    -- Make sure _G.coinsFake defaults to false if it's not already set
    if not _G.levelFake then
        _G.levelFake = false  -- กำหนดค่าเริ่มต้นให้เป็น false
    end

    -- Create a new thread to continuously check the toggle state
    task.spawn(function()
        while true do  -- Loop indefinitely
            task.wait(0.1)  -- Small delay to avoid performance issues

            if _G.levelFake then
                -- Get the player's coin value
            local player = game.Players.LocalPlayer
local stats = game:GetService("ReplicatedStorage"):WaitForChild("playerstats"):WaitForChild(player.Name):WaitForChild("Stats")
local level = stats:WaitForChild("level")

level.Value += _G.levelIncrease

            end
        end
    end)
end)


local Slider = Tabs.Fake:AddSlider("Slider", {
    Title = "levelIncrease",
    Description = "",
    Default = 2,
    Min = 1,
    Max = 750,
    Rounding = 1,
    Callback = function(Value)
        print("Slider was changed:", Value)
        _G.levelIncrease = Value  -- อัพเดทค่าการเพิ่ม coins จาก Slider
    end
})

Tabs.Fake:AddButton({
    Title = "level up",
    Description = "not loop",
    Callback = function()
 local player = game.Players.LocalPlayer
local stats = game:GetService("ReplicatedStorage"):WaitForChild("playerstats"):WaitForChild(player.Name):WaitForChild("Stats")
local level = stats:WaitForChild("level")

level.Value += _G.levelIncrease
    end
})


    local Toggle = Tabs.Trading:AddToggle("MyToggle", {
    Title = "No Trade Cooldown", 
    Default = false, 
    Description = "Trade with other player will have no cooldown."
})

Toggle:OnChanged(function(value)
    for _, playerModel in pairs(workspace:GetChildren()) do
        if playerModel:FindFirstChild("TradeOffer") then
            local tradeOffer = playerModel.TradeOffer
            if value then
                tradeOffer.HoldDuration = 0 -- เมื่อเปิด Toggle ตั้งเป็น 0 วินาที
            else
                tradeOffer.HoldDuration = 3 -- เมื่อปิด Toggle ตั้งเป็น 3 วินาที
            end
        end
    end
end)
local Backpack = game:GetService("Players").LocalPlayer.Backpack
local itemNames = {}
local itemCounts = {}

-- ดึงชื่อไอเท็มใน Backpack และนับจำนวนไอเท็มที่ซ้ำ
for _, item in ipairs(Backpack:GetChildren()) do
    if item:IsA("Tool") then
        local itemName = item.Name
        if not itemCounts[itemName] then
            itemCounts[itemName] = 1
            table.insert(itemNames, itemName)
        else
            itemCounts[itemName] = itemCounts[itemName] + 1
        end
    end
end
-- สร้าง Dropdown
local Dropdown = Tabs.Trading:AddDropdown("Dropdown", {
    Title = "Item Selector",
    Values = itemNames, -- ใช้ชื่อไอเท็มจาก Backpack
    Multi = false,
    Default = 1,
})

-- ตั้งค่าเริ่มต้นให้ Dropdown แสดงไอเท็มแรก
Dropdown:SetValue(itemNames[1])

-- Event เมื่อ Dropdown ถูกเปลี่ยนค่า
Dropdown:OnChanged(function(Value)
    print("Dropdown changed:", Value)
    -- ค้นหาไอเท็มที่เลือกใน Backpack
    local selectedItem = Backpack:FindFirstChild(Value)
    if selectedItem and selectedItem:IsA("Tool") then
        -- ทำการ Equip ไอเท็มที่เลือก
        local character = game:GetService("Players").LocalPlayer.Character
        if character then
            selectedItem.Parent = character
            game:GetService("Players").LocalPlayer.Character:WaitForChild("Humanoid"):EquipTool(selectedItem)
        end
    end
end)

function Rejoin_Server()
    local TeleportService = game:GetService("TeleportService")
        TeleportService:TeleportToPlaceInstance(game.PlaceId, game.JobId, game.Players.LocalPlayer)
end
function   Hop_Server()
local HttpService = game:GetService("HttpService")
local TeleportService = game:GetService("TeleportService")
local Players = game:GetService("Players")

local PlaceId = game.PlaceId -- กำหนดค่า PlaceId
local JobId = game.JobId -- กำหนดค่า JobId ปัจจุบัน

local function notify(title, message)
    game.StarterGui:SetCore("SendNotification", {
        Title = title;
        Text = message;
        Duration = 5;
    })
end

local function httpRequest(request)
    if syn and syn.request then
        return syn.request(request)
    elseif request and http and http.request then
        return http.request(request)
    else
        return nil
    end
end

if httpRequest then
    local servers = {}
    local req = httpRequest({
        Url = string.format("https://games.roblox.com/v1/games/%d/servers/Public?sortOrder=Desc&limit=100&excludeFullGames=true", PlaceId),
        Method = "GET"
    })

    if req and req.Body then
        local body = HttpService:JSONDecode(req.Body)

        if body and body.data then
            for _, v in ipairs(body.data) do
                if type(v) == "table" and tonumber(v.playing) and tonumber(v.maxPlayers) and v.playing < v.maxPlayers and v.id ~= JobId then
                    table.insert(servers, v.id)
                end
            end
        end
    end

    if #servers > 0 then
        local serverId = servers[math.random(1, #servers)]
        TeleportService:TeleportToPlaceInstance(PlaceId, serverId, Players.LocalPlayer)
    else
        notify("Serverhop", "Couldn't find a server.")
    end
else
    notify("Incompatible Exploit", "Your exploit does not support this command (missing request)")
end
end

Tabs.Server:AddButton({
    Title = "Rejoin Server",
    Description = "",
    Callback = function()
        Rejoin_Server()
    end
})

Tabs.Server:AddButton({
    Title = "Hop Server",
    Description = "",
    Callback = function()
        Hop_Server()
    end
})
local section = Tabs.Server:AddSection("Server id")

local JobIDInput = Tabs.Server:AddInput("JobIDInput", {
    Title = "Enter Job ID",
    Default = "",
    Placeholder = "Enter Job ID here...",
    Numeric = false, -- อนุญาตตัวเลขและข้อความ
    Finished = false, -- Callback จะถูกเรียกทุกครั้งที่พิมพ์
    Callback = function(Value)
    end
})

-- ตรวจจับการเปลี่ยนแปลงใน Input
JobIDInput:OnChanged(function()
end)

-- เพิ่ม Toggle เพื่อควบคุมการใช้งาน
local JoinServerToggle = Tabs.Server:AddToggle("JoinServerToggle", {
    Title = "Enable Join by Job ID",
    Default = false, -- ค่าเริ่มต้นของ Toggle
    Description = "enable joining the server Job ID."
})

-- เมื่อ Toggle ถูกเปลี่ยน
JoinServerToggle:OnChanged(function(Value)
    if Value then
        local jobId = JobIDInput.Value
        if jobId and jobId ~= "" then
            local TeleportService = game:GetService("TeleportService")
            local Players = game:GetService("Players")
            -- ใช้ TeleportService สำหรับเชื่อมต่อเซิร์ฟเวอร์
            TeleportService:TeleportToPlaceInstance(game.PlaceId, jobId, Players.LocalPlayer)
        end
    end
end)

Tabs.Server:AddButton({
    Title = "Copy Job ID",
    Description = "Copy server Job ID",
    Callback = function()
        local jobId = game.JobId

        -- คัดลอก Job ID ไปยังคลิปบอร์ด
        if setclipboard then
            setclipboard(jobId)
   end
end

})
local paragraphs = {
    Megalodon = Tabs.Event:AddParagraph({ Title = "Megalodon : Initializing...", Content = "" }),
    Isonade = Tabs.Event:AddParagraph({ Title = "Isonade : Initializing...", Content = "" })
}

local function updateFishStatus(fishName)
    pcall(function()
        while true do
            -- ตรวจสอบการมีอยู่ของปลา
            if workspace.zones.fishing:FindFirstChild(fishName) then
                paragraphs[fishName]:SetTitle(fishName .. " : ✅") -- แสดงสถานะว่าปลาพบ
            else
                paragraphs[fishName]:SetTitle(fishName .. " : ❌") -- แสดงสถานะว่าปลาไม่พบ
            end
            task.wait(0.5) -- อัพเดตทุก 0.5 วินาที
        end
    end)
end

-- เรียกใช้งานฟังก์ชันสำหรับปลาแต่ละตัว
for fishName, _ in pairs(paragraphs) do
    task.spawn(function()
        updateFishStatus(fishName)
    end)
end

 -- Dropdown สำหรับเลือก Event
local Dropdown = Tabs.Event:AddDropdown("Dropdown", {
    Title = "Teleport Event",
    Values = {"Isonade", "Megalodon Default"},
    Multi = false,
    Default = 1,
})

Dropdown:SetValue("Isonade")
Dropdown:SetValue("Megalodon Default")

Dropdown:OnChanged(function(Value)
    _G.Event = Value
end)
local running = false -- ตัวแปรควบคุมลูป
local createdPart -- ตัวแปรเก็บ Part ที่สร้าง

local Toggle = Tabs.Event:AddToggle("MyToggle", {
    Title = "Teleport To Event", 
    Default = false, 
    Description = "teleport to event."
})

Toggle:OnChanged(function(ToggleState)
    running = ToggleState -- อัพเดตสถานะการทำงาน

    if not running and createdPart then
        -- ลบ Part เมื่อปิด Toggle
        createdPart:Destroy()
        createdPart = nil
    end

    -- สร้างฟังก์ชันทำงานใน background
    spawn(function()
        while running and task.wait() do
            pcall(function()
                -- ตรวจสอบสถานะอีกครั้ง
                if running then
                    local target = workspace.zones.fishing:FindFirstChild(_G.Event)
                    if target then
                        local player = game.Players.LocalPlayer
                        local character = player.Character or player.CharacterAdded:Wait()
                        local humanoidRootPart = character:WaitForChild("HumanoidRootPart")

                        -- Teleport the player to 20 studs above the target
                        humanoidRootPart.CFrame = target.CFrame + Vector3.new(0, 120, 0)

                        -- ตรวจสอบว่ามีบล็อกเดิมอยู่หรือไม่ หากมีให้ลบก่อน
                        if createdPart then
                            createdPart:Destroy()
                            createdPart = nil
                        end

                        -- สร้างบล็อกสายรุ้งใหม่เหนือเป้าหมาย
                        createdPart = Instance.new("Part")
                        createdPart.Name = _G.Event .. "Block" -- ตั้งชื่อบล็อกตาม Event ที่เลือก
                        createdPart.Size = Vector3.new(15, 0, 15) -- ขนาดของบล็อก
                        createdPart.Position = target.Position + Vector3.new(0, 117, 0) -- วางบล็อกเหนือเป้าหมาย
                        createdPart.Anchored = true -- ทำให้บล็อกไม่เคลื่อนไหว
                        createdPart.Parent = workspace -- เพิ่มบล็อกเข้า workspace

                        -- เพิ่มฟังก์ชันเปลี่ยนสีสายรุ้ง
                        spawn(function()
                            while createdPart and createdPart.Parent and task.wait(0.1) do
                                local hue = tick() % 5 / 5 -- ใช้ tick() เพื่อวนค่าระหว่าง 0 ถึง 1
                                createdPart.Color = Color3.fromHSV(hue, 1, 1) -- เปลี่ยนสีตามค่า HSV
                            end
                        end)
                    end
                end
            end)
        end
    end)
end)

local section = Tabs.Event:AddSection("Megalodon Farm")

local Toggle = Tabs.Event:AddToggle("AutoMegalodonEvent", {
    Title = "Auto Megalodon Event",
    Default = false,
    Description = "Automatically search for the Megalodon Event by continuously using the Sundial Totem."
})
  Toggle:OnChanged(function(v)

_G.CFrameMegalodon = v
_G.PartMegalodon1 = v
_G.Totem = v
_G.Button = v
_G.CFrameMegalodon = false
_G.PartMegalodon1 = false
_G.Totem = false
_G.Button = false
_G.CFrameMegalodon = v
_G.PartMegalodon1 = v
_G.Totem = v
_G.Button = v
_G.Rod = v
_G.Rod = false
end)

local Toggle = Tabs.Event:AddToggle("AutoBuySundialTotem", {
    Title = "Auto Buy Sundial Totem",
    Default = false,
    Description = "Automatically purchase a Sundial Totem when it runs out."
})

    Toggle:OnChanged(function(v)

_G.ERER = v
_G.over =  v
_G.Totem =  v
_G.Button =  v
_G.over = false
_G.Totem = false
_G.Button = false
_G.ERER = v
_G.over =  v
_G.Totem =  v
_G.Button =  v

if not _G.ERER then
    _G.ERER = false  -- กำหนดค่าเริ่มต้นให้เป็น false
end

task.spawn(function()
    while true do  -- ลูปแบบต่อเนื่อง
        task.wait(0)  -- หยุดรอสั้นๆ เพื่อหลีกเลี่ยงการแฮงค์

        if _G.ERER then

local ReplicatedStorage = game:GetService("ReplicatedStorage")
local player = game.Players.LocalPlayer
local inventory = ReplicatedStorage.playerstats[player.Name].Inventory
local G = {}  -- สมมุติว่ามีตัวแปร G ที่คุณใช้

for _, item in pairs(inventory:GetChildren()) do
    if string.find(item.Name, "^Sundial Totem") then  -- ตรวจสอบว่าเริ่มต้นด้วย "Ancient Megalodon"
        if item:FindFirstChild("Stack") then
            local StackValue = item.Stack.Value
            if StackValue > 2 then
_G.over = false
_G.Totem = true
_G.Button = true

            elseif StackValue < 2 then
_G.over = true
_G.Totem = false
_G.Button = false

            elseif StackValue == 2 then
_G.over = true
_G.Totem = false
_G.Button = false
            end
            end
            end
end
end
end
end)


    end)

if not _G.CFrameMegalodon then
    _G.CFrameMegalodon = false  -- กำหนดค่าเริ่มต้นให้เป็น false
end

task.spawn(function()
    while true do  -- ลูปแบบต่อเนื่อง
        task.wait(0)  -- หยุดรอสั้นๆ เพื่อหลีกเลี่ยงการแฮงค์

        if _G.CFrameMegalodon then

local target = workspace.zones.fishing:FindFirstChild("Megalodon Default") -- ค้นหาเป้าหมาย

if target then
    -- ตรวจสอบว่ามี HumanoidRootPart ของผู้เล่น
    local player = game.Players.LocalPlayer
    local character = player.Character or player.CharacterAdded:Wait()
    local humanoidRootPart = character:WaitForChild("HumanoidRootPart")

    -- วาร์ปตัวละครไปยังตำแหน่งของเป้าหมาย
    humanoidRootPart.CFrame = target.CFrame * CFrame.new(0, 10, 0)  -- การยกตัวขึ้นเล็กน้อยจากตำแหน่งเป้าหมาย
end


end
end
end)



if not _G.PartMegalodon1 then
    _G.PartMegalodon1 = false  -- กำหนดค่าเริ่มต้นให้เป็น false
end

task.spawn(function()
    while true do  -- ลูปแบบต่อเนื่อง
        task.wait(3)  -- หยุดรอ 3 วินาที

        if _G.PartMegalodon1 then
            -- ค้นหาเป้าหมายใน workspace.zones.fishing
            local fishingZone = workspace.zones.fishing:FindFirstChild("Megalodon Default")

            -- ตรวจสอบว่าพบเป้าหมายหรือไม่
            if fishingZone then
                _G.Totem = false
_G.Button = false
_G.ERER = false     
_G.Rod = true

                local block = Instance.new("Part")
                block.Size = Vector3.new(4, 1, 4)  -- ขนาดบล็อก
                block.CFrame = fishingZone.CFrame * CFrame.new(0, 5, 0)  -- วางบล็อกด้านบนของเป้าหมาย
                block.Anchored = true  -- ทำให้บล็อกไม่ตก
                block.Color = Color3.fromRGB(255, 0, 0)  -- สีของบล็อก
                block.Parent = workspace  -- เพิ่มบล็อกลงใน workspace
                else
                _G.Totem = true
_G.Button = true
_G.ERER = true    
_G.Rod = false
            end
        end
    end
end)



if not _G.Totem then
    _G.Totem = false  -- กำหนดค่าเริ่มต้นให้เป็น false
end

task.spawn(function()
    while true do  -- ลูปแบบต่อเนื่อง
        task.wait(0)  -- หยุดรอสั้นๆ เพื่อหลีกเลี่ยงการแฮงค์

        if _G.Totem then

-- ตรวจสอบว่า "Sundial Totem" อยู่ใน Backpack ของผู้เล่น
local player = game:GetService("Players").LocalPlayer
local totem = player.Backpack:FindFirstChild("Sundial Totem")

-- ถ้าพบ "Sundial Totem" ใน Backpack
if totem then
    -- ตั้งค่าให้ "Sundial Totem" เป็นเครื่องมือที่ผู้เล่นถือ
    player.Character:WaitForChild("Humanoid"):EquipTool(totem)
 
end
end
end
end)




if not _G.Button then
    _G.Button = false  -- กำหนดค่าเริ่มต้นให้เป็น false
end

task.spawn(function()
    while true do  -- ลูปแบบต่อเนื่อง
        task.wait(1)  -- หยุดรอสั้นๆ เพื่อหลีกเลี่ยงการแฮงค์

        if _G.Button then
    game:GetService'VirtualUser':CaptureController()
    game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 670))
end
end
end)

if not _G.over then
    _G.over = false  -- กำหนดค่าเริ่มต้นให้เป็น false
end

task.spawn(function()
    while true do  -- ลูปแบบต่อเนื่อง
        task.wait(0)  -- หยุดรอสั้นๆ เพื่อหลีกเลี่ยงการแฮงค์

        if _G.over then
 game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1148, 135, -1075) 
game:service('VirtualInputManager'):SendKeyEvent(true, "E", false, game)
game:service('VirtualInputManager'):SendKeyEvent(false, "E", false, game)
local player = game:GetService("Players").LocalPlayer


local overPrompt = player.PlayerGui:FindFirstChild("over") and player.PlayerGui.over:FindFirstChild("prompt")
if overPrompt and overPrompt.confirm then
    local confirmButtonOver = overPrompt.confirm
    for _, connection in pairs(getconnections(confirmButtonOver.MouseButton1Click)) do
        connection.Function(confirmButtonOver)
    end
end
end
end
end)


  local section = Tabs.Enchant:AddSection("Enchant Relic")
local Dropdown = Tabs.Enchant:AddDropdown("Dropdown", {
    Title = "Dropdown",
    Values = {"Lucky", "Storming", "Mutated", "Noir", "Quality", "Resilient", "Scrapper", "Sea King", "Steady", "Swift", "Unbreakable", "Wormhole", "Abyssal", "Blessed", "Breezed", "Clever", "Controlled", "Divine", "Ghastly", "Hasty", "Insight", "Long"},
    Multi = false,
    Default = 1,
})

Dropdown:SetValue("Lucke") -- กำหนดค่าเริ่มต้น

Dropdown:OnChanged(function(Value)
    _G.enchant = Value -- เก็บค่า Enchant ที่เลือกไว้ใน `_G.enchant`
end)

_G.EnchantActive = false -- ตัวแปรสำหรับควบคุม Loop

function tp(x, y, z)
    local player = game.Players.LocalPlayer -- อ้างอิงผู้เล่นปัจจุบัน
    if player and player.Character and player.Character:FindFirstChild("HumanoidRootPart") then
        player.Character.HumanoidRootPart.CFrame = CFrame.new(Vector3.new(x, y, z)) -- เทเลพอร์ตไปยังตำแหน่งที่กำหนด
    else
        warn("ไม่พบตัวละครหรือ HumanoidRootPart")
    end
end

function Relic()
local player = game:GetService("Players").LocalPlayer
local backpack = player:WaitForChild("Backpack")

-- Loop เพื่อเช็คไอเทมใน Backpack
for _, item in pairs(backpack:GetChildren()) do
    if string.find(item.Name, "Relic") and item.Name ~= "Exalted Relic" then
        -- หากต้องการถือไอเทมนี้
        local humanoid = player.Character:FindFirstChildOfClass("Humanoid")
        if humanoid then
            humanoid:EquipTool(item)
        end
        break
    end
end
end

function E()
				game:service('VirtualInputManager'):SendKeyEvent(true, "E", false, game)
                task.wait(2)
				game:service('VirtualInputManager'):SendKeyEvent(false, "E", false, game)
end

function confirm()
    local playerGui = game:GetService("Players").LocalPlayer:WaitForChild("PlayerGui")
    
    -- Check if the GUI element "over" and its children exist
    if playerGui:FindFirstChild("over") and playerGui.over:FindFirstChild("prompt") then
        local prompt = playerGui.over.prompt
        
        -- Check if the "confirm" button exists
        if prompt:FindFirstChild("confirm") then
            -- Trigger the "MouseButton1Click" event for the confirmation button
            for _, connection in pairs(getconnections(prompt.confirm.MouseButton1Click)) do
                if connection.Function then
                    connection.Function()
                end
            end
        end
    end
end

function buy()
-- รันฟังก์ชัน InvokeServer ของ Merlin
local merlinPower = workspace.world.npcs.Merlin.Merlin.power

if merlinPower and merlinPower.InvokeServer then
    local success, result = pcall(function()
        return merlinPower:InvokeServer()
    end)

    if success then

    end
end
end


_G.AllRelic = false
spawn(function()
    while task.wait(2) do
        pcall(function()
            if _G.AllRelic then

        tp(1311, -802, -83)
        E()
        Relic()
        confirm()


            end
        end)
    end
end)



local Toggle = Tabs.Enchant:AddToggle("MyToggle", {
    Title = "Auto Enchant",
    Default = false,
    Description = "Enchant.",
})

Toggle:OnChanged(function(v)
    _G.AllRelic = v
    _G.EnchantActive = v -- ตั้งค่าตัวแปรตามสถานะ Toggle

    if v then -- ทำงานเมื่อ Toggle ถูกเปิดใช้งาน
        spawn(function()
            while _G.EnchantActive do -- เช็คสถานะของ Loop
                task.wait(0.2) -- ลดการใช้งานทรัพยากร
                pcall(function()
                    local player = game:GetService("Players").LocalPlayer
                    local backpack = player:WaitForChild("Backpack")

                    for _, item in pairs(backpack:GetChildren()) do
                        if string.find(item.Name, "Rod") then
                            
                            -- เข้าถึง GUI โดยใช้ชื่อของไอเท็ม
                            local enchantPath = player.PlayerGui:WaitForChild("hud")
                                :WaitForChild("safezone")
                                :WaitForChild("equipment")
                                :WaitForChild("rods")
                                :WaitForChild("scroll")
                                :WaitForChild("safezone")
                                :FindFirstChild(item.Name) -- ตรวจสอบ GUI สำหรับไอเท็มที่มีชื่อเดียวกัน

                            if enchantPath and enchantPath:FindFirstChild("enchant") then
                                local enchantValue = enchantPath.enchant.ContentText
                                if string.find(enchantValue, _G.enchant) then
                                    
                                    -- โค้ดสำหรับเทเลพอร์ตหรือทำงานอื่น
                                    _G.AllRelic = false -- ตัวอย่างการเทเลพอร์ต
                                end
                            end
                        end
                    end
                end)
            end
        end)
    end
end)


local Toggle = Tabs.Enchant:AddToggle("MyToggle", {
    Title = "Auto Buy Enchant Relic",
    Default = false,
    Description = "buy enchant relic.",
})

Toggle:OnChanged(function(v)
    _G.BuyRelic = v -- ตั้งค่าเปิด/ปิดฟีเจอร์
    spawn(function()
        while task.wait(0.5) do
            pcall(function()
                if _G.BuyRelic then

                tp(-932, 226, -991)
                buy()

                end
            end)
        end
    end)
end)
-- ตัวเลือกสำหรับการตั้งค่า UI (Theme)
local Dropdown = Tabs.Settings:AddDropdown("Dropdown", {
    Title = "Theme Ui",
    Values = { "Dark", "Darker", "Light", "Aqua", "Amethyst", "Rose" },
    Multi = false,
    Default = "Dark",
})

-- เปลี่ยนธีมตามค่าที่เลือก
Dropdown:OnChanged(function(Value)
    Fluent:SetTheme(Value)
end)

-- ตั้งค่าเริ่มต้นให้เป็นธีม "Dark"
Dropdown:SetValue("Aqua")


local Slider = Tabs.Settings:AddSlider("Slider", {
    Title = "Fps",
    Description = "",
    Default = 500,
    Min = 0,
    Max = 500,
    Rounding = 1,
    Callback = function(Value)
       setfpscap(Value)
    end
})

local section = Tabs.Shop:AddSection("Buy Rods")
local Dropdown = Tabs.Shop:AddDropdown("Dropdown", {
    Title = "Selector Rods",
    Values = { 
        "Long Rod [4500C$]", 
        "Fortune Rod [12750C$]", 
        "Aurora Rod [90000C$]", 
        "Midas Rod [55000C$]", 
        "Steady Rod [7000C$]", 
        "Rod Of The Depths [75000C$]", 
        "Training Rod [300C$]", 
        "Phoenix Rod [40000C$]", 
        "Avalanche Rod [35000C$]", 
        "Arctic Rod [25000C$]", 
        "Plastic Rod [900C$]", 
        "Magnet Rod [15000C$]", 
        "Rapid Rod [14000C$]", 
        "Flimsy Rod [0C$]", 
        "Fast Rod [4500C$]", 
        "Firework Rod [35000C$]", 
        "Scurvy Rod [50000C$]", 
        "Mythical Rod [110000C$]", 
        "Kings Rod [120000C$]", 
        "Carbon Rod [2000C$]", 
        "Summit Rod [300000C$]", 
        "Heaven's Rod [1750000C$]", 
        "Ice Warpers Rod [65000C$]", 
        "Crystalized Rod [35000C$]", 
        "Destiny Rod [190000C$]", 
        "Nocturnal Rod [11000C$]", 
        "Trident Rod [150000C$]", 
        "Reinforced Rod [20000C$]", 
        "Stone Rod [3000C$]", 
        "Lucky Rod [5250C$]"
    }, 
    Multi = false,
    Default = "Long Rod [4500C$]" -- ต้องให้ค่าตรงกับ Values
})

-- กำหนดค่าเริ่มต้นให้กับตัวเลือก
Dropdown:SetValue("Long Rod [4500C$]")

-- ฟังก์ชันอัพเดตค่า Dropdown เมื่อมีการเปลี่ยนแปลง
Dropdown:OnChanged(function(selected1)
    _G.SelectRod = selected1 -- อัปเดตค่าตัวแปรสำหรับเลือกคันเบ็ด
end)

Tabs.Shop:AddButton({
    Title = "Buy Rod",
    Description = "Buy selector rod.",
    Callback = function()
        local teleportPositions = {
            ["Long Rod [4500C$]"] = CFrame.new(482.74, 174.50, 148.02),
            ["Fortune Rod [12750C$]"] = CFrame.new(-1521.00, 141.48, 769.00),
            ["Aurora Rod [90000C$]"] = CFrame.new(-144.11, -513.07, 1129.53),
            ["Steady Rod [7000C$]"] = CFrame.new(-1514.31, 141.53, 761.31),
            ["Rod Of The Depths [75000C$]"] = CFrame.new(1704.82, -902.53, 1447.85),
            ["Training Rod [300C$]"] = CFrame.new(457.79, 154.40, 229.98),
            ["Phoenix Rod [40000C$]"] = CFrame.new(5970.14, 272.33, 852.93),
            ["Avalanche Rod [35000C$]"] = CFrame.new(19772.00, 415.44, 5418.57),
            ["Arctic Rod [25000C$]"] = CFrame.new(19578.46, 135.51, 5307.76),
            ["Plastic Rod [900C$]"] = CFrame.new(453.76, 150.50, 231.05),
            ["Magnet Rod [15000C$]"] = CFrame.new(-196.00, 132.50, 1931.00),
            ["Rapid Rod [14000C$]"] = CFrame.new(-1507.88, 141.85, 762.89),
            ["Flimsy Rod [0C$]"] = CFrame.new(471.40, 153.61, 229.33),
            ["Fast Rod [4500C$]"] = CFrame.new(447.31, 153.70, 219.57),
            ["Scurvy Rod [50000C$]"] = CFrame.new(-2827.49, 215.10, 1510.89),
            ["Kings Rod [120000C$]"] = CFrame.new(1377.49, -807.49, -301.67),
            ["Carbon Rod [2000C$]"] = CFrame.new(453.76, 153.49, 222.90),
            ["Summit Rod [300000C$]"] = CFrame.new(20208.63, 739.12, 5711.31),
            ["Heaven's Rod [1750000C$]"] = CFrame.new(20025.76, -473.59, 7147.43),
            ["Ice Warpers Rod [65000C$]"] = CFrame.new(19965.33, 589.20, 5551.95),
            ["Crystalized Rod [35000C$]"] = CFrame.new(19220.90, 395.87, 6058.30),
            ["Destiny Rod [190000C$]"] = CFrame.new(979.71, 131.32, -1235.08),
            ["Nocturnal Rod [11000C$]"] = CFrame.new(-143.80, -515.30, 1143.04),
            ["Trident Rod [150000C$]"] = CFrame.new(-1484.65, -223.49, -2195.60),
            ["Reinforced Rod [20000C$]"] = CFrame.new(-991.44, -244.73, -2689.97),
            ["Stone Rod [3000C$]"] = CFrame.new(5502.51, 146.77, -313.90),
            ["Lucky Rod [5250C$]"] = CFrame.new(445.53, 152.93, 221.11),
        }
    if _G.SelectRod then
            local targetPosition = teleportPositions[_G.SelectRod]
            if targetPosition then
                -- เก็บตำแหน่งปัจจุบันก่อนวาร์ป
                local currentPosition = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame

                -- วาร์ปไปยังตำแหน่งที่เลือก
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = targetPosition
                
                -- หน่วงเวลาเพื่อให้ตัวละครโหลดก่อนกดปุ่ม E
                task.wait(1) -- รอ 1 วินาที

                -- จำลองการกดปุ่ม "E"
                game:service('VirtualInputManager'):SendKeyEvent(true, "E", false, game)
                task.wait(0.5) -- รอเล็กน้อย
                game:service('VirtualInputManager'):SendKeyEvent(false, "E", false, game)

                -- ตรวจสอบ UI และกดปุ่มยืนยันถ้ามี
                task.wait(0.5) -- รอให้ UI ปรากฏ
                local playerGui = game:GetService("Players").LocalPlayer.PlayerGui
                if playerGui:FindFirstChild("over") and playerGui.over:FindFirstChild("prompt") then
                    local prompt = playerGui.over.prompt
                    if prompt:FindFirstChild("confirm") then
                        -- เรียกใช้งานปุ่มยืนยัน
                        for _, connection in pairs(getconnections(prompt.confirm.MouseButton1Click)) do
                            if connection.Function then
                                connection.Function()

                                -- วาร์ปกลับไปยังตำแหน่งเดิม
                                task.wait(0.5) -- รอให้การซื้อสำเร็จก่อนวาร์ปกลับ
                                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = currentPosition
                            end
                        end
                    end
                end
            end
        end
    end
})


local section = Tabs.Shop:AddSection("Buy Totem")
local Dropdown = Tabs.Shop:AddDropdown("Dropdown", {
    Title = "Selector Totem",
    Values = { 
        "Sundial Totem [2000C$]", 			
        "Smokescreen Totem [2000$]", 
        "Windset Totem [2000$]", 
        "Tempest Totem [2000$]", 
        "Aurora Totem [750000$]", 
        "Eclipse Totem [250000$]", 
        "Meteor Totem [75000C$]", 
        "Blizzard Totem [250000C$]", 
        "Avalanche Totem [150000$]", 
    }, 
    Multi = false,
    Default = "Long Rod [4500C$]" -- ต้องให้ค่าตรงกับ Values
})


-- ฟังก์ชันอัพเดตค่า Dropdown เมื่อมีการเปลี่ยนแปลง
Dropdown:OnChanged(function(selected2)
    _G.SelectTotem = selected2 -- อัปเดตค่าตัวแปรสำหรับเลือกคันเบ็ด
end)
Tabs.Shop:AddButton({
    Title = "Buy Totem",
    Description = "Buy selector totem.",
    Callback = function()
        local teleportPositions = {
            ["Sundial Totem [2000C$]"] = CFrame.new(-1147.37671, 134.5, -1074.64368),
            ["Smokescreen Totem [2000$]"] = CFrame.new(2791.70142, 139.729599, -629.47113),
            ["Windset Totem [2000$]"] = CFrame.new(2851.59619, 179.878937, 2703.08936),
            ["Tempest Totem [2000$]"] = CFrame.new(36.2399902, 135.413315, 1946.10913),
            ["Aurora Totem [750000$]"] = CFrame.new(-1812.42847, -136.927933, -3280.7124),
            ["Eclipse Totem [250000$]"] = CFrame.new(5969.2002, 274.111359, 839.5),
            ["Meteor Totem [75000C$]"] = CFrame.new(-1948.30005, 275.35672, 228.599991),
            ["Blizzard Totem [250000C$]"] = CFrame.new(20145, 742.952759, 5805),
            ["Avalanche Totem [150000$]"] = CFrame.new(19712.1152, 467.630585, 6054.31787),
        }

        for i = 1, tonumber(_G.Name) do
            wait(0.5) 

            if _G.SelectTotem then
                local targetPosition = teleportPositions[_G.SelectTotem]
                if targetPosition then
                    -- เก็บตำแหน่งปัจจุบันก่อนวาร์ป
                    local currentPosition = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame

                    -- วาร์ปไปยังตำแหน่งที่เลือก
                    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = targetPosition
                    
                    -- หน่วงเวลาเพื่อให้ตัวละครโหลดก่อนกดปุ่ม E
                    task.wait(0.005)

                    -- จำลองการกดปุ่ม "E"
                    game:service('VirtualInputManager'):SendKeyEvent(true, "E", false, game)
                    task.wait(0.005)
                    game:service('VirtualInputManager'):SendKeyEvent(false, "E", false, game)

                    -- ตรวจสอบ UI และกดปุ่มยืนยันถ้ามี
                    task.wait(0.1)
                    local playerGui = game:GetService("Players").LocalPlayer.PlayerGui
                    if playerGui:FindFirstChild("over") and playerGui.over:FindFirstChild("prompt") then
                        local prompt = playerGui.over.prompt
                        if prompt:FindFirstChild("confirm") then
                            for _, connection in pairs(getconnections(prompt.confirm.MouseButton1Click)) do
                                if connection.Function then
                                    connection.Function()
                                    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = currentPosition
                                end
                            end
                        end
                    end
                end
            end
        end
    end
})

-- ส่วนของ Input ที่รับค่าจำนวนรอบ
Tabs.Shop:AddInput("Input", {
    Title = "Totem Amount",
    Default = "5",  -- ค่าดีฟอลต์
    Placeholder = "",
    Numeric = true,
    Finished = false,
    Callback = function(value)
        _G.Name = tonumber(value) or 1  -- ตรวจสอบและกำหนดค่าเริ่มต้นหากไม่มีการป้อนค่า
    end
})

local SavedPositions = {}


-- ช่องป้อนชื่อไฟล์
local FileInput = Tabs.file:AddInput("FileNameInput", {
    Title = "Enter Name File",  -- แสดงเป็นภาษาไทย
    Default = "",
    Placeholder = "",
    Numeric = false,
    Finished = true -- กด Enter เพื่อบันทึกค่า
})

-- Dropdown for selecting files
local Dropdown = Tabs.file:AddDropdown("FileDropdown", {
    Title = "Select File",
    Values = {},
    Multi = false,
    Default = nil
})

-- Function to update Dropdown values
local function updateDropdown()
    local fileNames = {}
    for name, _ in pairs(SavedPositions) do
        table.insert(fileNames, name)
    end
    Dropdown:SetValues(fileNames)
end

-- Add new filename when pressing Enter
FileInput:OnChanged(function(Value)
    if Value and Value ~= "" and not SavedPositions[Value] then
        SavedPositions[Value] = {x = 0, y = 0, z = 0}
        updateDropdown()
    end
end)
-- Button to set current position
Tabs.file:AddButton({
    Title = "SetCF",
    Callback = function()
        local selectedFile = Dropdown.Value
        if selectedFile and SavedPositions[selectedFile] then
            local character = game.Players.LocalPlayer.Character
            if character and character:FindFirstChild("HumanoidRootPart") then
                local pos = character.HumanoidRootPart.Position
                SavedPositions[selectedFile] = {x = pos.X, y = pos.Y, z = pos.Z}
            end
        end
    end
})

-- Button to teleport to saved position
Tabs.file:AddButton({
    Title = "Teleport",
    Callback = function()
        local selectedFile = Dropdown.Value
        if selectedFile and SavedPositions[selectedFile] then
            local position = SavedPositions[selectedFile]
            local character = game.Players.LocalPlayer.Character
            if character and character:FindFirstChild("HumanoidRootPart") then
                character.HumanoidRootPart.CFrame = CFrame.new(position.x, position.y, position.z)
            end
        end
    end
})

-- Button to delete the selected file from the dropdown
Tabs.file:AddButton({
    Title = "Delete File All",
    Callback = function()
        local selectedFile = Dropdown.Value
        if selectedFile and SavedPositions[selectedFile] then
            SavedPositions[selectedFile] = nil -- Remove the selected file from the table
            updateDropdown() -- Update the dropdown list
            print("Deleted file:", selectedFile)
            Dropdown:SetValue(nil) -- Clear the dropdown selection
        end
    end
})















































































































































































































































































































































































































wait(2)
 local player = game:GetService("Players").LocalPlayer
local backpack = player.Backpack

-- Check for tools in the player's backpack
for _, item in pairs(backpack:GetChildren()) do
    if item:IsA("Tool") and string.find(item.Name, "Rod") then
        -- Ensure the item is not "Crab Cage" before equipping
        if item.Name ~= "Crab Cage" then
            local humanoid = player.Character:WaitForChild("Humanoid")
            humanoid:EquipTool(item)  -- Equip the rod item
            break  -- Stop searching after finding the first match
        end
    end
end

-- Check for tools in the player's character (not workspace.D3B3XxX)
local rodItem = nil
for _, item in pairs(player.Character:GetChildren()) do
    if item:IsA("Tool") and string.find(item.Name, "Rod") then
        -- Ensure the item is not "Crab Cage" before equipping
        if item.Name ~= "Crab Cage" then
            rodItem = item  -- Found the rod in the character, not the "Crab Cage"
            break  -- Stop searching after finding the first match
        end
    end
end
