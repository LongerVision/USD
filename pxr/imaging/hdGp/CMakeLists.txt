set(PXR_PREFIX pxr/imaging)
set(PXR_PACKAGE hdGp)

set(optionalPublicClasses "")

pxr_library(hdGp
    LIBRARIES
        hd
        hf
        ${TBB_tbb_LIBRARY}

    INCLUDE_DIRS
        ${TBB_INCLUDE_DIRS}

    PUBLIC_CLASSES
        generativeProcedural
        generativeProceduralPlugin
        generativeProceduralPluginRegistry
        generativeProceduralResolvingSceneIndex

    PRIVATE_CLASSES
        sceneIndexPlugin

    RESOURCE_FILES
        plugInfo.json
)
