#	$NetBSD: Makefile,v 1.14 2017/01/11 12:02:32 joerg Exp $

LIB=	clangAnalysis

.include <bsd.init.mk>

.PATH: ${CLANG_SRCDIR}/lib/Analysis

SRCS+=	AnalysisDeclContext.cpp \
	BodyFarm.cpp \
	CFG.cpp \
	CFGReachabilityAnalysis.cpp \
	CFGStmtMap.cpp \
	CallGraph.cpp \
	CloneDetection.cpp \
	CocoaConventions.cpp \
	CodeInjector.cpp \
	Consumed.cpp \
	Dominators.cpp \
	FormatString.cpp \
	LiveVariables.cpp \
	OSLog.cpp \
	ObjCNoReturn.cpp \
	PostOrderCFGView.cpp \
	ProgramPoint.cpp \
	PrintfFormatString.cpp \
	PseudoConstantAnalysis.cpp \
	ReachableCode.cpp \
	ScanfFormatString.cpp \
	ThreadSafety.cpp \
	ThreadSafetyCommon.cpp \
	ThreadSafetyLogical.cpp \
	ThreadSafetyTIL.cpp \
	UninitializedValues.cpp

.if defined(HOSTLIB)
.include <bsd.hostlib.mk>
.else
.include <bsd.lib.mk>
.endif
