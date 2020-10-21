---- Minecraft Crash Report ----
// I let you down. Sorry :(

Time: 10/21/20 6:52 AM
Description: Rendering overlay

java.lang.NullPointerException: Rendering overlay
	at net.minecraftforge.fml.config.ModConfig.getFullPath(ModConfig.java:98) ~[?:?] {re:classloading}
	at net.minecraftforge.fml.config.ConfigFileTypeHandler$ConfigLoadingException.<init>(ConfigFileTypeHandler.java:128) ~[?:?] {re:classloading}
	at net.minecraftforge.fml.config.ConfigFileTypeHandler.lambda$reader$1(ConfigFileTypeHandler.java:60) ~[?:?] {re:classloading}
	at net.minecraftforge.fml.config.ConfigFileTypeHandler$$Lambda$3482/92899392.apply(Unknown Source) ~[?:?] {}
	at net.minecraftforge.fml.config.ConfigTracker.openConfig(ConfigTracker.java:104) ~[?:?] {re:classloading}
	at net.minecraftforge.fml.config.ConfigTracker.lambda$loadConfigs$1(ConfigTracker.java:83) ~[?:?] {re:classloading}
	at net.minecraftforge.fml.config.ConfigTracker$$Lambda$3481/1588076648.accept(Unknown Source) ~[?:?] {}
	at java.lang.Iterable.forEach(Iterable.java:75) ~[?:1.8.0_51] {}
	at java.util.Collections$SynchronizedCollection.forEach(Collections.java:2062) ~[?:1.8.0_51] {}
	at net.minecraftforge.fml.config.ConfigTracker.loadConfigs(ConfigTracker.java:83) ~[?:?] {re:classloading}
	at net.minecraftforge.fml.ModLoader.lambda$null$18(ModLoader.java:201) ~[?:?] {re:classloading}
	at net.minecraftforge.fml.ModLoader$$Lambda$3480/294312200.run(Unknown Source) ~[?:?] {}
	at net.minecraftforge.fml.DistExecutor.unsafeRunWhenOn(DistExecutor.java:125) ~[?:?] {re:classloading}
	at net.minecraftforge.fml.ModLoader.loadMods(ModLoader.java:201) ~[?:?] {re:classloading}
	at net.minecraftforge.fml.client.ClientModLoader.lambda$startModLoading$7(ClientModLoader.java:132) ~[?:?] {re:classloading,pl:runtimedistcleaner:A}
	at net.minecraftforge.fml.client.ClientModLoader$$Lambda$3474/1637230255.run(Unknown Source) ~[?:?] {}
	at net.minecraftforge.fml.client.ClientModLoader.lambda$createRunnableWithCatch$4(ClientModLoader.java:123) ~[?:?] {re:classloading,pl:runtimedistcleaner:A}
	at net.minecraftforge.fml.client.ClientModLoader$$Lambda$2859/596299019.run(Unknown Source) ~[?:?] {}
	at net.minecraftforge.fml.client.ClientModLoader.startModLoading(ClientModLoader.java:132) ~[?:?] {re:classloading,pl:runtimedistcleaner:A}
	at net.minecraftforge.fml.client.ClientModLoader.lambda$onResourceReload$2(ClientModLoader.java:114) ~[?:?] {re:classloading,pl:runtimedistcleaner:A}
	at net.minecraftforge.fml.client.ClientModLoader$$Lambda$3468/1037793103.run(Unknown Source) ~[?:?] {}
	at net.minecraftforge.fml.client.ClientModLoader.lambda$createRunnableWithCatch$4(ClientModLoader.java:123) ~[?:?] {re:classloading,pl:runtimedistcleaner:A}
	at net.minecraftforge.fml.client.ClientModLoader$$Lambda$2859/596299019.run(Unknown Source) ~[?:?] {}
	at java.util.concurrent.CompletableFuture$AsyncRun.run(CompletableFuture.java:1618) ~[?:1.8.0_51] {}
	at java.util.concurrent.CompletableFuture$AsyncRun.exec(CompletableFuture.java:1610) ~[?:1.8.0_51] {}
	at java.util.concurrent.ForkJoinTask.doExec(ForkJoinTask.java:289) ~[?:1.8.0_51] {}
	at java.util.concurrent.ForkJoinPool$WorkQueue.runTask(ForkJoinPool.java:1056) ~[?:1.8.0_51] {}
	at java.util.concurrent.ForkJoinPool.runWorker(ForkJoinPool.java:1689) ~[?:1.8.0_51] {}
	at java.util.concurrent.ForkJoinWorkerThread.run(ForkJoinWorkerThread.java:157) ~[?:1.8.0_51] {}


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- Head --
Thread: Render thread
Stacktrace:
	at net.minecraftforge.fml.config.ModConfig.getFullPath(ModConfig.java:98) ~[?:?] {re:classloading}
	at net.minecraftforge.fml.config.ConfigFileTypeHandler$ConfigLoadingException.<init>(ConfigFileTypeHandler.java:128) ~[?:?] {re:classloading}
	at net.minecraftforge.fml.config.ConfigFileTypeHandler.lambda$reader$1(ConfigFileTypeHandler.java:60) ~[?:?] {re:classloading}
	at net.minecraftforge.fml.config.ConfigFileTypeHandler$$Lambda$3482/92899392.apply(Unknown Source) ~[?:?] {}
	at net.minecraftforge.fml.config.ConfigTracker.openConfig(ConfigTracker.java:104) ~[?:?] {re:classloading}
	at net.minecraftforge.fml.config.ConfigTracker.lambda$loadConfigs$1(ConfigTracker.java:83) ~[?:?] {re:classloading}
	at net.minecraftforge.fml.config.ConfigTracker$$Lambda$3481/1588076648.accept(Unknown Source) ~[?:?] {}
	at java.lang.Iterable.forEach(Iterable.java:75) ~[?:1.8.0_51] {}
	at java.util.Collections$SynchronizedCollection.forEach(Collections.java:2062) ~[?:1.8.0_51] {}
	at net.minecraftforge.fml.config.ConfigTracker.loadConfigs(ConfigTracker.java:83) ~[?:?] {re:classloading}
	at net.minecraftforge.fml.ModLoader.lambda$null$18(ModLoader.java:201) ~[?:?] {re:classloading}
	at net.minecraftforge.fml.ModLoader$$Lambda$3480/294312200.run(Unknown Source) ~[?:?] {}
	at net.minecraftforge.fml.DistExecutor.unsafeRunWhenOn(DistExecutor.java:125) ~[?:?] {re:classloading}
	at net.minecraftforge.fml.ModLoader.loadMods(ModLoader.java:201) ~[?:?] {re:classloading}
-- Overlay render details --
Details:
	Overlay name: net.minecraft.client.gui.ResourceLoadProgressGui
Stacktrace:
	at net.minecraft.client.renderer.GameRenderer.func_195458_a(GameRenderer.java:483) ~[?:?] {re:classloading,pl:accesstransformer:B,pl:runtimedistcleaner:A}
	at net.minecraft.client.Minecraft.func_195542_b(Minecraft.java:953) [?:?] {re:classloading,pl:accesstransformer:B,pl:runtimedistcleaner:A}
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:584) [?:?] {re:classloading,pl:accesstransformer:B,pl:runtimedistcleaner:A}
	at net.minecraft.client.main.Main.main(Main.java:184) [?:?] {re:classloading,pl:runtimedistcleaner:A}
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:1.8.0_51] {}
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:1.8.0_51] {}
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:1.8.0_51] {}
	at java.lang.reflect.Method.invoke(Method.java:497) ~[?:1.8.0_51] {}
	at net.minecraftforge.fml.loading.FMLClientLaunchProvider.lambda$launchService$0(FMLClientLaunchProvider.java:51) [forge-1.16.3-34.1.25.jar:34.1] {}
	at net.minecraftforge.fml.loading.FMLClientLaunchProvider$$Lambda$413/36627152.call(Unknown Source) [forge-1.16.3-34.1.25.jar:34.1] {}
	at cpw.mods.modlauncher.LaunchServiceHandlerDecorator.launch(LaunchServiceHandlerDecorator.java:37) [modlauncher-7.0.1.jar:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:54) [modlauncher-7.0.1.jar:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:72) [modlauncher-7.0.1.jar:?] {}
	at cpw.mods.modlauncher.Launcher.run(Launcher.java:81) [modlauncher-7.0.1.jar:?] {}
	at cpw.mods.modlauncher.Launcher.main(Launcher.java:65) [modlauncher-7.0.1.jar:?] {}


-- System Details --
Details:
	Minecraft Version: 1.16.3
	Minecraft Version ID: 1.16.3
	Operating System: Windows 8 (amd64) version 6.2
	Java Version: 1.8.0_51, Oracle Corporation
	Java VM Version: Java HotSpot(TM) 64-Bit Server VM (mixed mode), Oracle Corporation
	Memory: 1685047104 bytes (1606 MB) / 2080374784 bytes (1984 MB) up to 2147483648 bytes (2048 MB)
	CPUs: 4
	JVM Flags: 9 total; -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump -Xss1M -Xmx2G -XX:+UnlockExperimentalVMOptions -XX:+UseG1GC -XX:G1NewSizePercent=20 -XX:G1ReservePercent=20 -XX:MaxGCPauseMillis=50 -XX:G1HeapRegionSize=32M
	ModLauncher: 7.0.1+78+master.e9771d8
	ModLauncher launch target: fmlclient
	ModLauncher naming: srg
	ModLauncher services: 
		/mixin-0.8.2.jar mixin PLUGINSERVICE 
		/eventbus-3.0.3-service.jar eventbus PLUGINSERVICE 
		/forge-1.16.3-34.1.25.jar object_holder_definalize PLUGINSERVICE 
		/forge-1.16.3-34.1.25.jar runtime_enum_extender PLUGINSERVICE 
		/accesstransformers-2.2.0-shadowed.jar accesstransformer PLUGINSERVICE 
		/forge-1.16.3-34.1.25.jar capability_inject_definalize PLUGINSERVICE 
		/forge-1.16.3-34.1.25.jar runtimedistcleaner PLUGINSERVICE 
		/mixin-0.8.2.jar mixin TRANSFORMATIONSERVICE 
		/forge-1.16.3-34.1.25.jar fml TRANSFORMATIONSERVICE 
	FML: 34.1
	Forge: net.minecraftforge:34.1.25
	FML Language Providers: 
		javafml@34.1
		minecraft@1
	Mod List: 
		forge-1.16.3-34.1.25-client.jar Minecraft {minecraft@1.16.3 COMMON_SETUP}
		forge-1.16.3-34.1.25-universal.jar Forge {forge@34.1.25 COMMON_SETUP}
	Crash Report UUID: 7e887f7c-035a-4cb5-8365-e564f8dcdbec
	Launched Version: 1.16.3-forge-34.1.25
	Backend library: LWJGL version 3.2.2 build 10
	Backend API: Intel(R) HD Graphics 4600 GL version 4.3.0 - Build 20.19.15.5126, Intel
	GL Caps: Using framebuffer using OpenGL 3.0
	Using VBOs: Yes
	Is Modded: Definitely; Client brand changed to 'forge'
	Type: Client (map_client.txt)
	Graphics mode: fancy
	Resource Packs: 
	Current Language: English (US)
	CPU: 4x Intel(R) Core(TM) i5-4300M CPU @ 2.60GHz
