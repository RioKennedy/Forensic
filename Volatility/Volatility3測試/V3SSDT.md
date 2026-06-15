# 測試內容

- .\vol.exe -f .\OtterCTF.vmem windows.ssdt.SSDT

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.ssdt.SSDT
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Index   Address Module  Symbol

0       0xf80002ee0ca0  ntoskrnl        NtMapUserPhysicalPagesScatter
1       0xf80002dc88c0  ntoskrnl        NtWaitForSingleObject
2       0xf80002aca1a0  ntoskrnl        NtCallbackReturn
3       0xf80002dbba80  ntoskrnl        NtReadFile
4       0xf80002ded7a0  ntoskrnl        NtDeviceIoControlFile
5       0xf80002de49a0  ntoskrnl        NtWriteFile
6       0xf80002d8ec90  ntoskrnl        NtRemoveIoCompletion
7       0xf80002d88220  ntoskrnl        NtReleaseSemaphore
8       0xf80002de5fc4  ntoskrnl        NtReplyWaitReceivePort
9       0xf80002eb0a40  ntoskrnl        NtReplyPort
10      0xf80002d9b770  ntoskrnl        NtSetInformationThread
11      0xf80002dbb010  ntoskrnl        NtSetEvent
12      0xf80002dc9b10  ntoskrnl        NtClose
13      0xf80002db3530  ntoskrnl        NtQueryObject
14      0xf80002db0360  ntoskrnl        NtQueryInformationFile
15      0xf80002dac910  ntoskrnl        NtOpenKey
16      0xf80002db2760  ntoskrnl        NtEnumerateValueKey
17      0xf80002dc4b60  ntoskrnl        NtFindAtom
18      0xf80002d80350  ntoskrnl        NtQueryDefaultLocale
19      0xf80002da22e0  ntoskrnl        NtQueryKey
20      0xf80002da34d0  ntoskrnl        NtQueryValueKey
21      0xf80002dc9c90  ntoskrnl        NtAllocateVirtualMemory
22      0xf80002de3410  ntoskrnl        NtQueryInformationProcess
23      0xf80002df6fa0  ntoskrnl        NtWaitForMultipleObjects32
24      0xf80002f28f30  ntoskrnl        NtWriteFileGather
25      0xf80002dc059c  ntoskrnl        NtSetInformationProcess
26      0xf80002d86170  ntoskrnl        NtCreateKey
27      0xf80002abf4d0  ntoskrnl        NtFreeVirtualMemory
28      0xf80002f0f580  ntoskrnl        NtImpersonateClientOfPort
29      0xf80002dc8404  ntoskrnl        NtReleaseMutant
30      0xf80002d985c0  ntoskrnl        NtQueryInformationToken
31      0xf80002de59c0  ntoskrnl        NtRequestWaitReplyPort
32      0xf80002dac930  ntoskrnl        NtQueryVirtualMemory
33      0xf80002da6338  ntoskrnl        NtOpenThreadToken
34      0xf80002dbfa30  ntoskrnl        NtQueryInformationThread
35      0xf80002da52ec  ntoskrnl        NtOpenProcess
36      0xf80002db0cb0  ntoskrnl        NtSetInformationFile
37      0xf80002deb9e0  ntoskrnl        NtMapViewOfSection
38      0xf80002db60a0  ntoskrnl        NtAccessCheckAndAuditAlarm
39      0xf80002de9ad4  ntoskrnl        NtUnmapViewOfSection
40      0xf80002de5fe0  ntoskrnl        NtReplyWaitReceivePortEx
41      0xf80002d8b5a4  ntoskrnl        NtTerminateProcess
42      0xf80002ee5980  ntoskrnl        NtSetEventBoostPriority
43      0xf80002d3a6c4  ntoskrnl        NtReadFileScatter
44      0xf80002da5d80  ntoskrnl        NtOpenThreadTokenEx
45      0xf80002dadc40  ntoskrnl        NtOpenProcessTokenEx
46      0xf80002d83150  ntoskrnl        NtQueryPerformanceCounter
47      0xf80002d8a670  ntoskrnl        NtEnumerateKey
48      0xf80002dbb0dc  ntoskrnl        NtOpenFile
49      0xf80002dc89d4  ntoskrnl        NtDelayExecution
50      0xf80002dbb7b0  ntoskrnl        NtQueryDirectoryFile
51      0xf80002ddc8fc  ntoskrnl        NtQuerySystemInformation
52      0xf80002debd80  ntoskrnl        NtOpenSection
53      0xf80002ee5520  ntoskrnl        NtQueryTimer
54      0xf80002dac870  ntoskrnl        NtFsControlFile
55      0xf80002d79850  ntoskrnl        NtWriteVirtualMemory
56      0xf80002da8c3c  ntoskrnl        NtCloseObjectAuditAlarm
57      0xf80002dabc10  ntoskrnl        NtDuplicateObject
58      0xf80002dade20  ntoskrnl        NtQueryAttributesFile
59      0xf80002dbc588  ntoskrnl        NtClearEvent
60      0xf80002d799c0  ntoskrnl        NtReadVirtualMemory
61      0xf80002db3e44  ntoskrnl        NtOpenEvent
62      0xf80002d87334  ntoskrnl        NtAdjustPrivilegesToken
63      0xf80002d78b08  ntoskrnl        NtDuplicateToken
64      0xf80002ad4140  ntoskrnl        NtContinue
65      0xf80002e7d450  ntoskrnl        NtQueryDefaultUILanguage
66      0xf80002db6efc  ntoskrnl        NtQueueApcThread
67      0xf80002aa1568  ntoskrnl        NtYieldExecution
68      0xf80002d2506c  ntoskrnl        NtAddAtom
69      0xf80002d97e60  ntoskrnl        NtCreateEvent
70      0xf80002de6fc0  ntoskrnl        NtQueryVolumeInformationFile
71      0xf80002dad9b0  ntoskrnl        NtCreateSection
72      0xf80002d71700  ntoskrnl        NtFlushBuffersFile
73      0xf80002db2a34  ntoskrnl        NtApphelpCacheControl
74      0xf80002f42f20  ntoskrnl        NtCreateProcessEx
75      0xf80002eb0b70  ntoskrnl        NtCreateThread
76      0xf80002ee5fd0  ntoskrnl        NtIsProcessInJob
77      0xf80002deab2c  ntoskrnl        NtProtectVirtualMemory
78      0xf80002deedb0  ntoskrnl        NtQuerySection
79      0xf80002dc31c8  ntoskrnl        NtResumeThread
80      0xf80002da8530  ntoskrnl        NtTerminateThread
81      0xf80002f36a10  ntoskrnl        NtReadRequestData
82      0xf80002dda400  ntoskrnl        NtCreateFile
83      0xf80002d6c284  ntoskrnl        NtQueryEvent
84      0xf80002f36990  ntoskrnl        NtWriteRequestData
85      0xf80002dec900  ntoskrnl        NtOpenDirectoryObject
86      0xf80002d73ba4  ntoskrnl        NtAccessCheckByTypeAndAuditAlarm
87      0xf80002e59ea0  ntoskrnl        NtQuerySystemTime
88      0xf80002dc8f58  ntoskrnl        NtWaitForMultipleObjects
89      0xf80002d6e96c  ntoskrnl        NtSetInformationObject
90      0xf80002ee4e10  ntoskrnl        NtCancelIoFile
91      0xf80002ab7c2c  ntoskrnl        NtTraceEvent
92      0xf80002d8ee3c  ntoskrnl        NtPowerInformation
93      0xf80002d861b0  ntoskrnl        NtSetValueKey
94      0xf80002a8746c  ntoskrnl        NtCancelTimer
95      0xf80002abf0a4  ntoskrnl        NtSetTimer
96      0xf80002d8c2e0  ntoskrnl        NtAcceptConnectPort
97      0xf80002a98ad4  ntoskrnl        NtAccessCheck
98      0xf80002aad4d4  ntoskrnl        NtAccessCheckByType
99      0xf80002be7e20  ntoskrnl        NtAccessCheckByTypeResultList
100     0xf80002ef7560  ntoskrnl        NtAccessCheckByTypeResultListAndAuditAlarm
101     0xf80002ef74a0  ntoskrnl        NtAccessCheckByTypeResultListAndAuditAlarmByHandle
102     0xf80002f14030  ntoskrnl        NtAddBootEntry
103     0xf80002f13d90  ntoskrnl        NtAddDriverEntry
104     0xf80002d522e0  ntoskrnl        NtAdjustGroupsToken
105     0xf80002ef9080  ntoskrnl        NtAlertResumeThread
106     0xf80002db9d4c  ntoskrnl        NtAlertThread
107     0xf80002d69d80  ntoskrnl        NtAllocateLocallyUniqueId
108     0xf80002eb0020  ntoskrnl        NtAllocateReserveObject
109     0xf80002f27480  ntoskrnl        NtAllocateUserPhysicalPages
110     0xf80002d1fb20  ntoskrnl        NtAllocateUuids
111     0xf80002daf730  ntoskrnl        NtAlpcAcceptConnectPort
112     0xf80002d3a15c  ntoskrnl        NtAlpcCancelMessage
113     0xf80002db45dc  ntoskrnl        NtAlpcConnectPort
114     0xf80002dba428  ntoskrnl        NtAlpcCreatePort
115     0xf80002d6f7a4  ntoskrnl        NtAlpcCreatePortSection
116     0xf80002dba870  ntoskrnl        NtAlpcCreateResourceReserve
117     0xf80002d6ea10  ntoskrnl        NtAlpcCreateSectionView
118     0xf80002d73524  ntoskrnl        NtAlpcCreateSecurityContext
119     0xf80002d66b44  ntoskrnl        NtAlpcDeletePortSection
120     0xf80002ea12d0  ntoskrnl        NtAlpcDeleteResourceReserve
121     0xf80002d8b7fc  ntoskrnl        NtAlpcDeleteSectionView
122     0xf80002d736f0  ntoskrnl        NtAlpcDeleteSecurityContext
123     0xf80002d8b290  ntoskrnl        NtAlpcDisconnectPort
124     0xf80002da5b50  ntoskrnl        NtAlpcImpersonateClientOfPort
125     0xf80002db532c  ntoskrnl        NtAlpcOpenSenderProcess
126     0xf80002d8e7a0  ntoskrnl        NtAlpcOpenSenderThread
127     0xf80002d63180  ntoskrnl        NtAlpcQueryInformation
128     0xf80002da56c0  ntoskrnl        NtAlpcQueryInformationMessage
129     0xf80002ea1150  ntoskrnl        NtAlpcRevokeSecurityContext
130     0xf80002ddf6c0  ntoskrnl        NtAlpcSendWaitReceivePort
131     0xf80002db9490  ntoskrnl        NtAlpcSetInformation
132     0xf80002d1f850  ntoskrnl        NtAreMappedFilesTheSame
133     0xf80002d89cd4  ntoskrnl        NtAssignProcessToJobObject
134     0xf80002df5fd0  ntoskrnl        NtCancelIoFileEx
135     0xf80002ef9e70  ntoskrnl        NtCancelSynchronousIoFile
136     0xf80002efb470  ntoskrnl        NtCommitComplete
137     0xf80002f22000  ntoskrnl        NtCommitEnlistment
138     0xf80002d60220  ntoskrnl        NtCommitTransaction
139     0xf80002efeef0  ntoskrnl        NtCompactKeys
140     0xf80002d97730  ntoskrnl        NtCompareTokens
141     0xf80002d5ca00  ntoskrnl        CmBcbCacheTrimNotification
141     0xf80002d5ca00  ntoskrnl        EmFalseCallback
141     0xf80002d5ca00  ntoskrnl        ExpDummyGetAtomTable
141     0xf80002d5ca00  ntoskrnl        FsRtlSyncVolumes
141     0xf80002d5ca00  ntoskrnl        IopPnPAddDevice
141     0xf80002d5ca00  ntoskrnl        NtCompleteConnectPort
141     0xf80002d5ca00  ntoskrnl        TmpOpenTransactionManager
141     0xf80002d5ca00  ntoskrnl        xHalGetInterruptTranslator
142     0xf80002f501f0  ntoskrnl        NtCompressKey
143     0xf80002d80148  ntoskrnl        NtConnectPort
144     0xf80002eafda0  ntoskrnl        NtCreateDebugObject
145     0xf80002d697c0  ntoskrnl        NtCreateDirectoryObject
146     0xf80002d58d78  ntoskrnl        NtCreateEnlistment
147     0xf80002eaff20  ntoskrnl        NtCreateEventPair
148     0xf80002db4d30  ntoskrnl        NtCreateIoCompletion
149     0xf80002eb06a0  ntoskrnl        NtCreateJobObject
150     0xf80002ef5350  ntoskrnl        NtCreateJobSet
151     0xf80002d5b8e8  ntoskrnl        NtCreateKeyTransacted
152     0xf80002d8528c  ntoskrnl        NtCreateKeyedEvent
153     0xf80002d46450  ntoskrnl        NtCreateMailslotFile
154     0xf80002d78e40  ntoskrnl        NtCreateMutant
155     0xf80002d93fe0  ntoskrnl        NtCreateNamedPipeFile
156     0xf80002f3a1c0  ntoskrnl        NtCreatePagingFile
157     0xf80002d8e73c  ntoskrnl        NtCreatePort
158     0xf80002d43cc4  ntoskrnl        NtCreatePrivateNamespace
159     0xf80002f42fb0  ntoskrnl        NtCreateProcess
160     0xf80002ef7360  ntoskrnl        NtCreateProfile
161     0xf80002ef7430  ntoskrnl        NtCreateProfileEx
162     0xf80002d5cbf8  ntoskrnl        NtCreateResourceManager
163     0xf80002d79344  ntoskrnl        NtCreateSemaphore
164     0xf80002d69e00  ntoskrnl        NtCreateSymbolicLinkObject
165     0xf80002dc2128  ntoskrnl        NtCreateThreadEx
166     0xf80002d67038  ntoskrnl        NtCreateTimer
167     0xf80002d68d5c  ntoskrnl        NtCreateToken
168     0xf80002d55fe0  ntoskrnl        NtCreateTransaction
169     0xf80002d5bff0  ntoskrnl        NtCreateTransactionManager
170     0xf80002d7d4a0  ntoskrnl        NtCreateUserProcess
171     0xf80002ef0d60  ntoskrnl        NtCreateWaitablePort
172     0xf80002db4e38  ntoskrnl        NtCreateWorkerFactory
173     0xf80002f201f0  ntoskrnl        NtDebugActiveProcess
174     0xf80002ef7b90  ntoskrnl        NtDebugContinue
175     0xf80002f09f00  ntoskrnl        NtDeleteAtom
176     0xf80002ec2fa0  ntoskrnl        NtDeleteBootEntry
177     0xf80002ec2a80  ntoskrnl        NtDeleteDriverEntry
178     0xf80002d2c780  ntoskrnl        NtDeleteFile
179     0xf80002d531d0  ntoskrnl        NtDeleteKey
180     0xf80002ef66d0  ntoskrnl        NtDeleteObjectAuditAlarm
181     0xf80002df2ef0  ntoskrnl        NtDeletePrivateNamespace
182     0xf80002d51b1c  ntoskrnl        NtDeleteValueKey
183     0xf80002ea0ec0  ntoskrnl        NtDisableLastKnownGood
184     0xf80002f29890  ntoskrnl        NtDisplayString
185     0xf80002bef2b0  ntoskrnl        NtDrawText
186     0xf80002eed770  ntoskrnl        NtEnableLastKnownGood
187     0xf80002f2f3a0  ntoskrnl        NtEnumerateBootEntries
188     0xf80002f2e980  ntoskrnl        NtEnumerateDriverEntries
189     0xf80002f2f960  ntoskrnl        NtEnumerateSystemEnvironmentValuesEx
190     0xf80002ef4e00  ntoskrnl        NtEnumerateTransactionObject
191     0xf80002f01c70  ntoskrnl        NtExtendSection
192     0xf80002df636c  ntoskrnl        NtFilterToken
193     0xf80002f056a0  ntoskrnl        NtFlushInstallUILanguage
194     0xf80002d438c4  ntoskrnl        NtFlushInstructionCache
195     0xf80002d726ac  ntoskrnl        NtFlushKey
196     0xf80002a72898  ntoskrnl        NtFlushProcessWriteBuffers
197     0xf80002d37370  ntoskrnl        NtFlushVirtualMemory
198     0xf80002e3ee50  ntoskrnl        NtFlushWriteBuffer
199     0xf80002efbb60  ntoskrnl        NtFreeUserPhysicalPages
200     0xf80002bc9cb0  ntoskrnl        NtFreezeRegistry
201     0xf80002ef8f90  ntoskrnl        NtFreezeTransactions
202     0xf80002d21ae8  ntoskrnl        NtGetContextThread
203     0xf80002d621e0  ntoskrnl        NtGetCurrentProcessorNumber
204     0xf80002ef3db0  ntoskrnl        NtGetDevicePowerState
205     0xf80002d850a0  ntoskrnl        NtGetMUIRegistryInfo
206     0xf80002f022a0  ntoskrnl        NtGetNextProcess
207     0xf80002f01fb0  ntoskrnl        NtGetNextThread
208     0xf80002f00ef0  ntoskrnl        NtGetNlsSectionPtr
209     0xf80002ef8e10  ntoskrnl        NtGetNotificationResourceManager
210     0xf80002d3d320  ntoskrnl        NtGetPlugPlayEvent
211     0xf80002a728a8  ntoskrnl        NtGetWriteWatch
212     0xf80002d67220  ntoskrnl        NtImpersonateAnonymousToken
213     0xf80002d796d4  ntoskrnl        NtImpersonateThread
214     0xf80002d7a228  ntoskrnl        NtInitializeNlsFiles
215     0xf80002d2b740  ntoskrnl        NtInitializeRegistry
216     0xf80002f1b140  ntoskrnl        NtInitiatePowerAction
217     0xf80002e3d620  ntoskrnl        NtIsSystemResumeAutomatic
218     0xf80002d92d10  ntoskrnl        NtIsUILanguageComitted
219     0xf80002eff2b0  ntoskrnl        NtListenPort
220     0xf80002f4b4f0  ntoskrnl        NtLoadDriver
221     0xf80002d50594  ntoskrnl        NtLoadKey
222     0xf80002f509a0  ntoskrnl        NtLoadKey2
223     0xf80002d4f5a4  ntoskrnl        NtLoadKeyEx
224     0xf80002d46b9c  ntoskrnl        NtLockFile
225     0xf80002ee6ad0  ntoskrnl        NtLockProductActivationKeys
226     0xf80002efe5e0  ntoskrnl        NtLockRegistryKey
227     0xf80002be41d0  ntoskrnl        NtLockVirtualMemory
228     0xf80002f078d0  ntoskrnl        NtMakePermanentObject
229     0xf80002d6bb58  ntoskrnl        NtMakeTemporaryObject
230     0xf80002d7b610  ntoskrnl        NtMapCMFModule
231     0xf80002ee14b0  ntoskrnl        NtMapUserPhysicalPages
232     0xf80002f14000  ntoskrnl        NtModifyBootEntry
233     0xf80002f13d60  ntoskrnl        NtModifyDriverEntry
234     0xf80002d3820c  ntoskrnl        NtNotifyChangeDirectoryFile
235     0xf80002d88144  ntoskrnl        NtNotifyChangeKey
236     0xf80002d87884  ntoskrnl        NtNotifyChangeMultipleKeys
237     0xf80002ef9ab0  ntoskrnl        NtNotifyChangeSession
238     0xf80002ef1e90  ntoskrnl        NtOpenEnlistment
239     0xf80002eb7d90  ntoskrnl        NtOpenEventPair
240     0xf80002eb7a10  ntoskrnl        NtOpenIoCompletion
241     0xf80002eb7f00  ntoskrnl        NtOpenJobObject
242     0xf80002da3c90  ntoskrnl        NtOpenKeyEx
243     0xf80002ef58a0  ntoskrnl        NtOpenKeyTransacted
244     0xf80002d5bd00  ntoskrnl        NtOpenKeyTransactedEx
245     0xf80002eb7ce0  ntoskrnl        NtOpenKeyedEvent
246     0xf80002debe04  ntoskrnl        NtOpenMutant
247     0xf80002ef67e0  ntoskrnl        NtOpenObjectAuditAlarm
248     0xf80002d6ae74  ntoskrnl        NtOpenPrivateNamespace
249     0xf80002d78f70  ntoskrnl        NtOpenProcessToken
250     0xf80002df58ec  ntoskrnl        NtOpenResourceManager
251     0xf80002d39f68  ntoskrnl        NtOpenSemaphore
252     0xf80002eb7980  ntoskrnl        NtOpenSession
253     0xf80002d79060  ntoskrnl        NtOpenSymbolicLinkObject
254     0xf80002dc473c  ntoskrnl        NtOpenThread
255     0xf80002eb7e50  ntoskrnl        NtOpenTimer
256     0xf80002ef1bf0  ntoskrnl        NtOpenTransaction
257     0xf80002ef4ae0  ntoskrnl        NtOpenTransactionManager
258     0xf80002d96b3c  ntoskrnl        NtPlugPlayControl
259     0xf80002efb5d0  ntoskrnl        NtPrePrepareComplete
260     0xf80002f220b0  ntoskrnl        NtPrePrepareEnlistment
261     0xf80002efb680  ntoskrnl        NtPrepareComplete
262     0xf80002f22160  ntoskrnl        NtPrepareEnlistment
263     0xf80002d6c040  ntoskrnl        NtPrivilegeCheck
264     0xf80002ef6fd0  ntoskrnl        NtPrivilegeObjectAuditAlarm
265     0xf80002d3c764  ntoskrnl        NtPrivilegedServiceAuditAlarm
266     0xf80002f285e0  ntoskrnl        NtPropagationComplete
267     0xf80002ef9600  ntoskrnl        NtPropagationFailed
268     0xf80002d371c0  ntoskrnl        NtPulseEvent
269     0xf80002f2f100  ntoskrnl        NtQueryBootEntryOrder
270     0xf80002ec2c80  ntoskrnl        NtQueryBootOptions
271     0xf80002b0d720  ntoskrnl        NtQueryDebugFilterState
272     0xf80002dec344  ntoskrnl        NtQueryDirectoryObject
273     0xf80002f2ee60  ntoskrnl        NtQueryDriverEntryOrder
274     0xf80002f37780  ntoskrnl        NtQueryEaFile
275     0xf80002d640d4  ntoskrnl        NtQueryFullAttributesFile
276     0xf80002ec49e0  ntoskrnl        NtQueryInformationAtom
277     0xf80002ef0150  ntoskrnl        NtQueryInformationEnlistment
278     0xf80002f11710  ntoskrnl        NtQueryInformationJobObject
279     0xf80002ea0df0  ntoskrnl        NtQueryInformationPort
280     0xf80002eef820  ntoskrnl        NtQueryInformationResourceManager
281     0xf80002eefa90  ntoskrnl        NtQueryInformationTransaction
282     0xf80002df5460  ntoskrnl        NtQueryInformationTransactionManager
283     0xf80002be6510  ntoskrnl        NtQueryInformationWorkerFactory
284     0xf80002d911c0  ntoskrnl        NtQueryInstallUILanguage
285     0xf80002e4f0a0  ntoskrnl        NtQueryIntervalProfile
286     0xf80002ee5110  ntoskrnl        NtQueryIoCompletion
287     0xf80002db6f28  ntoskrnl        NtQueryLicenseValue
288     0xf80002d86d44  ntoskrnl        NtQueryMultipleValueKey
289     0xf80002ee5690  ntoskrnl        NtQueryMutant
290     0xf80002f1ced0  ntoskrnl        NtQueryOpenSubKeys
291     0xf80002f1cae0  ntoskrnl        NtQueryOpenSubKeysEx
292     0xf80002e3d3c0  ntoskrnl        NtQueryPortInformationProcess
293     0xf80002f36a90  ntoskrnl        NtQueryQuotaInformationFile
294     0xf80002d96940  ntoskrnl        NtQuerySecurityAttributesToken
295     0xf80002d67350  ntoskrnl        NtQuerySecurityObject
296     0xf80002ee5840  ntoskrnl        NtQuerySemaphore
297     0xf80002d7d27c  ntoskrnl        NtQuerySymbolicLinkObject
298     0xf80002f143d0  ntoskrnl        NtQuerySystemEnvironmentValue
299     0xf80002f389a0  ntoskrnl        NtQuerySystemEnvironmentValueEx
300     0xf80002db4c90  ntoskrnl        NtQuerySystemInformationEx
301     0xf80002d3881c  ntoskrnl        NtQueryTimerResolution
302     0xf80002db6dc0  ntoskrnl        NtQueueApcThreadEx
303     0xf80002ad4380  ntoskrnl        NtRaiseException
304     0xf80002f012a0  ntoskrnl        NtRaiseHardError
305     0xf80002efb520  ntoskrnl        NtReadOnlyEnlistment
306     0xf80002f21050  ntoskrnl        NtRecoverEnlistment
307     0xf80002d59828  ntoskrnl        NtRecoverResourceManager
308     0xf80002d59410  ntoskrnl        NtRecoverTransactionManager
309     0xf80002f286f0  ntoskrnl        NtRegisterProtocolAddressInformation
310     0xf80002ee60c0  ntoskrnl        NtRegisterThreadTerminatePort
311     0xf80002db9820  ntoskrnl        NtReleaseKeyedEvent
312     0xf80002abeaac  ntoskrnl        NtReleaseWorkerFactoryWorker
313     0xf80002d71324  ntoskrnl        NtRemoveIoCompletionEx
314     0xf80002ee53b0  ntoskrnl        NtRemoveProcessDebug
315     0xf80002f23440  ntoskrnl        NtRenameKey
316     0xf80002f11540  ntoskrnl        NtRenameTransactionManager
317     0xf80002f4fab0  ntoskrnl        NtReplaceKey
318     0xf80002bf4e90  ntoskrnl        NtReplacePartitionUnit
319     0xf80002ec0cd0  ntoskrnl        NtReplyWaitReplyPort
320     0xf80002dc48e0  ntoskrnl        NtRequestPort
321     0xf80002ee5a00  ntoskrnl        NtResetEvent
322     0xf80002a72440  ntoskrnl        NtResetWriteWatch
323     0xf80002f4fd90  ntoskrnl        NtRestoreKey
324     0xf80002f1e560  ntoskrnl        NtResumeProcess
325     0xf80002ef96a0  ntoskrnl        NtRollbackComplete
326     0xf80002f1a3a0  ntoskrnl        NtRollbackEnlistment
327     0xf80002f206f0  ntoskrnl        NtRollbackTransaction
328     0xf80002f22210  ntoskrnl        NtRollforwardTransactionManager
329     0xf80002f4dd00  ntoskrnl        NtSaveKey
330     0xf80002f4da50  ntoskrnl        NtSaveKeyEx
331     0xf80002f4d880  ntoskrnl        NtSaveMergedKeys
332     0xf80002d7e5f4  ntoskrnl        NtSecureConnectPort
333     0xf80002ea4c10  ntoskrnl        NtSerializeBoot
334     0xf80002f13dc0  ntoskrnl        NtSetBootEntryOrder
335     0xf80002ec5040  ntoskrnl        NtSetBootOptions
336     0xf80002d21410  ntoskrnl        NtSetContextThread
337     0xf80002ea0fc0  ntoskrnl        NtSetDebugFilterState
338     0xf80002ea5150  ntoskrnl        NtSetDefaultHardErrorPort
339     0xf80002e7d4d0  ntoskrnl        NtSetDefaultLocale
340     0xf80002e7ebb0  ntoskrnl        NtSetDefaultUILanguage
341     0xf80002f13b20  ntoskrnl        NtSetDriverEntryOrder
342     0xf80002f37300  ntoskrnl        NtSetEaFile
343     0xf80002ef89a0  ntoskrnl        NtSetHighEventPair
344     0xf80002ef9150  ntoskrnl        NtSetHighWaitLowEventPair
345     0xf80002ef56d0  ntoskrnl        NtSetInformationDebugObject
346     0xf80002ef50a0  ntoskrnl        NtSetInformationEnlistment
347     0xf80002f1d1f0  ntoskrnl        NtSetInformationJobObject
348     0xf80002d744c0  ntoskrnl        NtSetInformationKey
349     0xf80002f282c0  ntoskrnl        NtSetInformationResourceManager
350     0xf80002d677b8  ntoskrnl        NtSetInformationToken
351     0xf80002f29a60  ntoskrnl        NtSetInformationTransaction
352     0xf80002f114a0  ntoskrnl        NtSetInformationTransactionManager
353     0xf80002ac1df0  ntoskrnl        NtSetInformationWorkerFactory
354     0xf80002e7aaf0  ntoskrnl        NtSetIntervalProfile
355     0xf80002d64010  ntoskrnl        NtSetIoCompletion
356     0xf80002ee4fd0  ntoskrnl        NtSetIoCompletionEx
357     0xf80002b57210  ntoskrnl        CcTestControl
357     0xf80002b57210  ntoskrnl        NtSetLdtEntries
357     0xf80002b57210  ntoskrnl        PspQueryDescriptorThread
357     0xf80002b57210  ntoskrnl        PspQueryLdtInformation
357     0xf80002b57210  ntoskrnl        PspSetLdtInformation
357     0xf80002b57210  ntoskrnl        PspSetLdtSize
357     0xf80002b57210  ntoskrnl        PspSetProcessIoHandlers
357     0xf80002b57210  ntoskrnl        xHalAllocateMapRegisters
357     0xf80002b57210  ntoskrnl        xKdReleasePciDeviceForDebugging
357     0xf80002b57210  ntoskrnl        xKdSetupPciDeviceForDebugging
358     0xf80002ef8a10  ntoskrnl        NtSetLowEventPair
359     0xf80002ef91d0  ntoskrnl        NtSetLowWaitHighEventPair
360     0xf80002f390c0  ntoskrnl        NtSetQuotaInformationFile
361     0xf80002d6e538  ntoskrnl        NtSetSecurityObject
362     0xf80002f14060  ntoskrnl        NtSetSystemEnvironmentValue
363     0xf80002f38680  ntoskrnl        NtSetSystemEnvironmentValueEx
364     0xf80002f461a0  ntoskrnl        NtSetSystemInformation
365     0xf80002d1b450  ntoskrnl        NtSetSystemPowerState
366     0xf80002eec2b0  ntoskrnl        NtSetSystemTime
367     0xf80002f16650  ntoskrnl        NtSetThreadExecutionState
368     0xf80002a807c4  ntoskrnl        NtSetTimerEx
369     0xf80002ef77a0  ntoskrnl        NtSetTimerResolution
370     0xf80002f27f00  ntoskrnl        NtSetUuidSeed
371     0xf80002df5040  ntoskrnl        NtSetVolumeInformationFile
372     0xf80002f51db0  ntoskrnl        NtShutdownSystem
373     0xf80002d88dd8  ntoskrnl        NtShutdownWorkerFactory
374     0xf80002be0ee0  ntoskrnl        NtSignalAndWaitForSingleObject
375     0xf80002f21f50  ntoskrnl        NtSinglePhaseReject
376     0xf80002f30ab0  ntoskrnl        NtStartProfile
377     0xf80002efc360  ntoskrnl        NtStopProfile
378     0xf80002f1fc30  ntoskrnl        NtSuspendProcess
379     0xf80002d21930  ntoskrnl        NtSuspendThread
380     0xf80002d63ab0  ntoskrnl        NtSystemDebugControl
381     0xf80002d30890  ntoskrnl        NtTerminateJobObject
382     0xf80002dc476c  ntoskrnl        NtTestAlert
383     0xf80002bc9f40  ntoskrnl        NtThawRegistry
384     0xf80002ea65c0  ntoskrnl        NtThawTransactions
385     0xf80002d780a0  ntoskrnl        NtTraceControl
386     0xf80002ef63c0  ntoskrnl        NtTranslateFilePath
387     0xf80002e57310  ntoskrnl        NtUmsThreadYield
388     0xf80002eb8dc0  ntoskrnl        NtUnloadDriver
389     0xf80002d5eb40  ntoskrnl        NtUnloadKey
390     0xf80002d56ea4  ntoskrnl        NtUnloadKey2
391     0xf80002f21730  ntoskrnl        NtUnloadKeyEx
392     0xf80002d467fc  ntoskrnl        NtUnlockFile
393     0xf80002be0410  ntoskrnl        NtUnlockVirtualMemory
394     0xf80002f35cd0  ntoskrnl        NtVdmControl
395     0xf80002f093d0  ntoskrnl        NtWaitForDebugEvent
396     0xf80002db9ab4  ntoskrnl        NtWaitForKeyedEvent
397     0xf80002abe2a0  ntoskrnl        NtWaitForWorkViaWorkerFactory
398     0xf80002eef600  ntoskrnl        NtWaitHighEventPair
399     0xf80002eef690  ntoskrnl        NtWaitLowEventPair
400     0xf80002ac6750  ntoskrnl        NtWorkerFactoryWorkerReady
```


# windows.ssdt.SSDT 分析

## 1. Plugin 功能說明

`windows.ssdt.SSDT` 用來列出 Windows 系統中的 SSDT（System Service Descriptor Table）項目。

SSDT 是 Windows Kernel 用來處理系統呼叫的重要結構，許多 Windows API 最後會透過 SSDT 進入核心層執行。

在 Rootkit 或惡意驅動程式分析中，攻擊者可能會修改 SSDT，使某些系統呼叫被導向惡意 Driver，以達到隱藏 Process、隱藏檔案、攔截系統行為或繞過安全檢查的目的。

因此，`SSDT` Plugin 可用來檢查是否存在可疑的 SSDT Hook。

---

## 2. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.ssdt.SSDT
```

---

## 3. 欄位說明

| 欄位        | 說明        |
| --------- | --------- |
| `Index`   | SSDT 項目編號 |
| `Address` | 系統呼叫函式位址  |
| `Module`  | 該函式所屬模組   |
| `Symbol`  | 函式名稱      |

---

## 4. 執行結果摘要

本次結果列出多個 SSDT 系統呼叫項目，例如：

```text
NtOpenProcess
NtCreateFile
NtReadFile
NtWriteFile
NtQuerySystemInformation
NtAllocateVirtualMemory
NtProtectVirtualMemory
NtCreateThreadEx
NtLoadDriver
NtUnloadDriver
NtTerminateProcess
```

這些都是 Windows 常見的 Kernel System Call。

從結果觀察，大部分項目的 `Module` 都是：

```text
ntoskrnl
```

`ntoskrnl` 是 Windows NT Kernel 的核心模組，屬於正常系統元件。

---

## 5. 重要觀察

本次 SSDT 結果中沒有看到明顯異常的模組，例如：

```text
unknown
UNKNOWN
可疑 Driver 名稱
非 Windows 系統模組
與 Rick And Morty 或 vmware-tray.exe 相關的模組
```

例如以下系統呼叫皆指向 `ntoskrnl`：

```text
NtOpenProcess
NtCreateFile
NtReadFile
NtWriteFile
NtQuerySystemInformation
NtAllocateVirtualMemory
NtProtectVirtualMemory
NtCreateThreadEx
NtTerminateProcess
```

這表示目前沒有觀察到 SSDT 被可疑 Driver 攔截或 Hook 的明顯跡象。

---

## 6. 鑑識判斷

SSDT Hook 常見於 Kernel Rootkit，用來隱藏惡意活動，例如：

```text
隱藏 Process
隱藏檔案
隱藏 Registry Key
攔截系統呼叫
干擾防毒或鑑識工具
```

但本次 `SSDT` 結果中，SSDT 項目主要仍指向 `ntoskrnl`，沒有發現明顯被未知 Driver 或可疑模組替換的情況。

因此，目前沒有證據顯示本案存在 SSDT Hook 或 Kernel Rootkit 行為。
