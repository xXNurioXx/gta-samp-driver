cmake_minimum_required(VERSION 3.16)
project(gta_sa_self_driver_bot)

set(CMAKE_CXX_STANDARD 20)

add_executable(
        gta_sa_self_driver_bot
        main.cpp

        application/Console.cpp

        math/MathTrigonometry.cpp
        math/AxisManager.cpp

        game/GameResources.cpp
        game/MemoryReader.cpp
        game/GameUtils.cpp

        drivers/Walker.cpp
        drivers/Driver.cpp
        drivers/Checkpoint.cpp

        interactions/CaptchaSolver.cpp
        interactions/ChatManager.cpp
        interactions/Movement.cpp

        routes/miners/Miner.cpp
        routes/miners/IronMiner.cpp
        routes/miners/CopperMiner.cpp
        routes/miners/TitaniumMiner.cpp
        routes/miners/MercuryMiner.cpp

        routes/fishermans/Fisherman.cpp
        routes/fishermans/DolphinFisherman.cpp
        routes/fishermans/TurtleFisherman.cpp
)