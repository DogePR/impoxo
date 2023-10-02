local whitelist={"EarthyDeathChef","1245","1241","124142"}
game.Players.PlayerAdded:Connect(function(p)
    local found=false
    for i,v in pairs(whitelist) do
        if v==p.Name then
            found=true
        end
    end
    if found==false then
        p:Kick()
    end
end)
