
include_directories (${PROJECT_SOURCE_DIR}/pink ${PROJECT_SOURCE_DIR}/graphcuts )

add_library(pink
            lattribheight.c   
            llabelextrema.c 
            lppm2GA.c
            lwshedtopo.c
            lderiche.c
            lhierarchie.c
            jccodimage.c
            jcimage.c
            jcgraphes.c
            jccomptree.c
            jclabelextrema.c
            llpeGA.c
            lga2khalimsky.c
            mcrbt.c
            mccodimage.c
            mccomptree.c
            mcfahsalembier.c  
            mcimage.c         
            mcindic.c         
            mclifo.c          
            mcfifo.c
            mcunionfind.c
            mtrand64.c 
            kruskal.c
            prim.c
            mincover.c
            MSF_utils.c
	    mcweightgraph.c
	    sjcomptree.c
	    mcsort.c
	    overlap.c
	    decisionSegmentation.c
)
	     
set (CMAKE_C_FLAGS "-fpic -g -DUNIXIO")
target_link_libraries(pink)
